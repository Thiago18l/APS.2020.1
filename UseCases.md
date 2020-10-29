<h2 align="center">Modelo de caso de Uso</h2><br>


<h2 align="center">Diagrama de caso de Uso</h2>
<hr>
<a align="center">
<img src="https://i.imgur.com/2hQa5gk.png" alt="Diagrama de caso de uso"/>
</a>
<hr/>

## Documentação de caso de uso

### 1. ESPECIFICAÇÃO DE CASO DE USO
<p>1.1) Identificação do caso de uso - CDU001 - Logar no Sistema</p>

a) **Ator principal**: Usuário

b) **Pré-condições**: É preciso estar cadastrado no sistema.

c) **Resumo**: Este caso de uso descreve as etapas percorridas pelo o usuário para logar-se ao sistema

d) **Cenário Principal**:

| Ações do ator        | Resposta do Sistema           
| :------------- |:-------------:
|1. Selecionar a opção de logar    |  |
| | 2. Apresentar o formulário de login
|3. Informar login e senha |
| | 4. Autenticar cliente

e) **Cenário alternativo - Usuário login ou senha incorretos:**

| Ações do ator        | Resposta do Sistema           
| :------------- |:-------------:|
|1. Selecionar a opção de logar    |  |
| | 2. Apresentar o formulário de login
|3. Informar login e senha |
| | 4. Autenticar cliente
| | 5. Informar que os dados não conferem
| | 6. Solicitar novamente os dados
|7. Informar login e senha|
| |8. Autenticar cliente

<p>1.2 Identificação de caso de uso - CDU002 - Gerar relatório</p>

a) **Ator principal**: Gestor geral

b) **Resumo**: Este caso detalha os passos para que o gestor geral possa gerar relatórios e anexar documentos ao relatório em questão

c) **Cenário Principal**: 

| Ações do ator | Resposta do Sistema
| :----------- | :-------------:|
|1.Selecionar a opção de gerar relatório |
| |2.Apresentar formulário de relatório
|3. Preencher os dados para popular o relatório |
| | 4. Verificar se os campos do formulário não estão em branco
||  5. Abrir uma tela de busca para encontrar o arquivo que o usuário deseja anexar
|6. Selecionar anexos |
| |7.Informar opções de envio
|8. Selecionar opção de envio |
| | 9. Enviar relatório

d) **Cenário Alternativo - relatório sem nenhum preenchimento**:

| Ações do ator | Resposta do Sistema
| :----------- | :-------------:|
|1.Selecionar a opção de gerar relatório |
| |2. Apresentar formulário de relatório
|3. Não inseriu nenhum dado no formulário |
| |4. Verificar se os campos do formulário não estão em branco
|| 5. Informar que não foi preenchido nenhum campo do formulário
| |6. Apresentar formulário de relatório
|7. Preencher os dados para popular o relatório |
||8. Verificar se os campos do formulário não estão em branco
||9. Abir uma tela de buscar para encontrar o arquivo que o usuário deseja anexar
|10. Selecionar anexos |
||11.Informar opções de envio
|12. Selecionar opção de envio|
||13. Enviar relatório

<p>1.3 Identificação de caso de uso - CDU003 - Cadastrar assuntos</p>

a) **Ator principal**: Gestor geral

b) **Resumo**: Este caso detalha como o usuário irá cadastrar assuntos para reuniões e pautas.

c) **Cenário principal**:

| Ações do ator | Resposta do Sistema
| :----------- | :-------------:|
|1.Selecionar a opção de cadastrar assunto |
| |2.Apresentar formulário de cadastro de assuntos
| |3.Solicitar um título para o assunto
|4. Informar título |
| |5. Solicitar data para agendamento
|6. Informar data |
||7.Solicitar se o usuário deseja salvar
|8. Salvar assunto |

d) **Cenário alternativo - Gestor não informou um título**:
| Ações do ator | Resposta do Sistema
| :----------- | :-------------:|
|1.Selecionar a opção de cadastrar assunto |
||2.Apresentar formulário de cadastro de assuntos
||3.Solicitar um título para o assunto
||4.Usuário não informou um título
||5.Informar que um assunto precisa de um título
||6.Solicitar um título para o assunto
|7. Informar título |
| |8. Solicitar data para agendamento
|9. Informar data |
||10.Solicitar se o usuário deseja salvar
|11. Salvar assunto |

e) **Cenário alternativo - Gestor não informou uma data**:

| Ações do ator | Resposta do Sistema
| :----------- | :-------------:|
|1.Selecionar a opção de cadastrar assunto |
| |2.Apresentar formulário de cadastro de assuntos
| |3.Solicitar um título para o assunto
|4. Informar título |
||5. Solicitar data para agendamento
||6.Usuário não informou uma data
||7.Informar que para cadastrar um assunto necessita uma data
||8.Solicitar data para agendamento
|9. Informar data|
||10.Solicitar se o usuário deseja salvar
|11. Salvar assunto|