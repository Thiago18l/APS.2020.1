## Estudo da parte de Segurança do SQL Server
#### Como gerenciamos acesso?
 - Concedendo, Revogando e Negando;
 - Tipos de Autenticação;
 - Cargos do server;

 #### Como será identificado os Objetos mais acessados:

 Existente no SQL Server desde 2005 existe a view chamada `sys.procedures`, trata-se de um objeto de sistema que possibilita o acesso às informações relativas a **stored procedures**. A partir dessa view é possível não apenas obter dados como o nome das procedures presentes em uma base de dados.

 Além de que existe a ferramenta de auditória dentro do proprio SQL SERVER que gera logs com dados que queremos.

#### Tabelas mais utilizadas: 

O script abaixo descobre a data e a hora do último acesso de uma tabela ou view:

```sql
SELECT
    A.name AS [object_name],
    A.type_desc,
    B.database_id,
    C.name AS index_name,
    (
        SELECT MAX(Ultimo_Acesso)
        FROM (VALUES (B.last_user_seek),(B.last_user_scan),(B.last_user_lookup),(B.last_user_update)) AS DataAcesso(Ultimo_Acesso)
    ) AS last_access,
    B.last_user_seek,
    B.last_user_scan,
    B.last_user_lookup,
    B.last_user_update,
    NULLIF(
        (CASE WHEN B.last_user_seek IS NOT NULL THEN 'Seek, ' ELSE '' END) +
        (CASE WHEN B.last_user_scan IS NOT NULL THEN 'Scan, ' ELSE '' END) +
        (CASE WHEN B.last_user_lookup IS NOT NULL THEN 'Lookup, ' ELSE '' END) +
        (CASE WHEN B.last_user_update IS NOT NULL THEN 'Update, ' ELSE '' END)
    , '') AS operations
FROM
    sys.objects                                 A
    LEFT JOIN sys.dm_db_index_usage_stats       B	ON	B.[object_id] = A.[object_id] AND B.[database_id] = DB_ID()
    LEFT JOIN sys.indexes                       C	ON	C.index_id = B.index_id AND C.[object_id] = B.[object_id]
WHERE
    A.[type_desc] IN ('VIEW', 'USER_TABLE')
ORDER BY
    A.name,
    B.index_id
    
```

Utilizando DMV (Dynamic Management Views) para saber a quantidade de sessões por usuário:

```sql
SELECT login_name,
COUNT(session_id) AS session_count
FROM sys.dm_exec_sessions
GROUP BY login_name;
```

Referência : [Microsoft Documentation](https://docs.microsoft.com/en-us/sql/relational-databases/system-dynamic-management-views/sys-dm-exec-sessions-transact-sql?redirectedfrom=MSDN&view=sql-server-ver15)