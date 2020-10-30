**PROJETO**: Sistema de gerenciamento do laboratório de robótica

**CLIENTE**: Disciplina de Análise e projeto de sistemas (APS)

# Histórico de Versões

| Data        | Versão           | Descrição | Autor
| :------------- |:-------------:| :-----------: | :-----:
| 03/08/2020      | 1.0 | Criação e preenchimento do documento | Thiago Lopes 
| 21/10/2020| 2.0 | Ínicio da criação dos casos de uso| Thiago Lopes
| 28/10/2020| 2.1 | Refatoração do diagrama de caso de uso| Thiago Lopes
| 29/10/2020| 2.2 | Aperfeiçoamento das especificações dos casos de uso| Thiago Lopes

# Sumário

1. [Diagrama de caso de uso](#diagram)
2. [Identificação dos Casos de uso](#identificacao)
3. [Especificações de casos de uso](#espc)
    - 3.1 - [Logar no Sistema](#login)
    - 3.2 - [Gerar Relatório](#relatorio)
    - 3.3 - [Cadastrar assuntos](#assuntos)
    - 3.4 - [Cadastrar demandas](#demandas)
    - 3.5 - [Registrar saída de materiais](#saida)
    - 3.6 - [Registrar entrada de materiais](#entrada)
    - 3.7 - [Aluno cadastra demandas](#aluno)

<hr>


## <a name="diagram">1. Diagrama de caso de Uso</a>
<hr>
<a align="center">
<img src="https://i.imgur.com/2hQa5gk.png" alt="Diagrama de caso de uso"/>
</a>
<hr/>


## <a name="identificacao">2.Identificação dos casos de uso</a>
 - **CDU001** - O usuário pode realizar login no sistema
 - **CDU002** - O Gestor gera relatórios
 - **CDU003** - O Gestor cadastra assuntos
 - **CDU004** - O Gestor cadastra demandas
 - **CDU005** - O Gestor registra saída de materiais
 - **CDU006** - O Gestor registrar entrada de materiais
 - **CDU007** - Aluno pode cadastrar demandas no sistema

### 3. <a name="espc">ESPECIFICAÇÕES DE CASOS DE USO</a>

<hr>

<h3><a name="login">3.1 Identificação do caso de uso - <strong>CDU001</strong> - Logar no Sistema</a></h3>

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

<h3><a name="relatorio">3.2 Identificação de caso de uso - <b>CDU002</b> - Gerar relatório</a></h3>

a) **Ator principal**: Gestor geral

b) **Resumo**: Este caso detalha os passos para que o gestor geral possa gerar relatórios e anexar documentos ao relatório em questão

c) **Pré-condições**: O gestor geral necessita gerar um relatório com base nos dados do sistema

d) **Cenário Principal - Gestor gera um relatório**: 

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

e) **Cenário Alternativo I - relatório sem nenhum preenchimento**:

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

<h3><a name="assuntos">3.3 Identificação de caso de uso - <b>CDU003</b> - Cadastrar assuntos</a></h3>

a) **Ator principal**: Gestor geral

b) **Resumo**: Este caso detalha como o usuário irá cadastrar assuntos para reuniões e pautas.

c) **Cenário principal - Gestor cadastra um assunto no sistema**:

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

d) **Cenário alternativo I - Gestor não informou um título**:
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

d) **Cenário alternativo II - Gestor não informou uma data**:

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


<h3><a name="demandas">3.4 Identificação de caso de uso - <b>CDU004</b> - Cadastrar Demandas</a></h3>

a) **Ator principal**: Gestor geral

b) **Resumo**: Este caso detalha como o usuário irá cadastrar demandas dentro do sistema para que possa haver um controle dos itens dentro do laboratório.

c) **Pré-condição**: ter materiais cadastrados dentro do sistema

d) **Cenário principal - Gestor cadastra uma demanda**:

| Ações do ator | Resposta do Sistema
| :----------- | :-------------:|
|1. Selecionar a opção de cadastrar Demandas |
||2.Apresentar formulário de cadastro de Demandas
||3.Solicitar um título para cadastrar a demanda
|4. Informar título |
|5. Popular o formulário|
||6. Informar materiais cadastrados
||7. Verificar materiais no banco
|8. Selecionar material|
||9. Informar que o material foi vinculado a demanda
|10.Salvar demanda |
||11. Informar que a demanda foi cadastrada

e) **Cenário alternativo I - Nenhum material cadastrado no sistema**:
| Ações do ator | Resposta do Sistema
| :----------- | :-------------:|
|1. Selecionar a opção de cadastrar Demandas |
||2.Apresentar formulário de cadastro de Demandas
||3.Solicitar um título para cadastrar a demanda
|4. Informar título |
|5. Popular o formulário|
||6. Informar materiais cadastrados
||7. Verificar materiais no banco
||8. Informar que não existe nenhum material na base de dados
||9.Solicitar para que cadastre um material no sistema
||10.Retornar para o menu principal

e) **Cenário alternativo II - Gestor não informou um título**:

| Ações do ator | Resposta do Sistema
| :----------- | :-------------:|
|1. Selecionar a opção de cadastrar Demandas |
||2.Apresentar formulário de cadastro de Demandas
||3.Solicitar um título para cadastrar a demanda
||4.Gestor não informou um título
||5.Informar que uma demanda necessita de um título
||6.Solicitar um título para a demanda
|7. Informar título|
|8. Popular o formulário|
||9.Informar materiais cadastrados
||10.Verificar materiais no banco
|11.Selecionar material|
||12.Informar que o material foi vinculado a demanda
|13.Salvar demanda|
||14.Informar que a demanda foi cadastrada

e) **Cenário alternativo III - Gestor não preencheu o formulário**:
| Ações do ator | Resposta do Sistema
| :----------- | :-------------:|
|1. Selecionar a opção de cadastrar Demandas |
||2.Apresentar formulário de cadastro de Demandas
||3.Solicitar um título para cadastrar a demanda
|4.Informar título|
|5.Preencher formulário|
||5.Verificar se o formulário não está em branco
||6.Informar que o formulário deve ser preenchido
||7.Apresentar formulário de cadastro de Demandas
|8. Preencher formulário|
||9.Verificar se o formulário não está em branco
||10.Informar  materiais cadastrados
||11.Verificar materiais no banco
|12. Selecionar material|
||13.Informar que o material foi vinculado a demanda
|14.Salvar demanda|
||15.Informar que a demanda foi cadastrada


<h3><a name="saida">3.5 Identificação de caso de uso - <b>CDU005</b> - Registrar saída de materiais</a></h3>

a) **Ator principal**: Gestor geral

b) **Resumo**: Este caso detalha os passos para que o gestor geral possa registrar a saída de materiais do laboratório de robótica.

c) **Pré-condição**: retirada de algum material do laboratório

d) **Cenário Principal - Registrar saída de materiais**:

| Ações do ator | Resposta do Sistema
| :----------- | :-------------:|
|1.Selecionar a opção de registrar saída de materiais|
||2.Apresentar formulário para preencher quais materiais foram retirados
|3. Preencher formulário|
|4. Seleciona a opção de registrar|
||5.Solicitar confirmação
||6. Registra a saída dos materiais

e) **Cenário alternativo - Gestor não preencheu o formulário**:
| Ações do ator | Resposta do Sistema
| :----------- | :-------------:|
|1.Selecionar a opção de registrar saída de materiais|
||2.Apresentar formulário para preencher quais materiais foram retirados
|3. Não preencheu os campos|
|4. Seleciona a opção de registrar|
||5.Verifica se o formulário não esta em branco
||6.Informar que o formulário deve ser preenchido
||7. Apresentar formulário
|8. Preenche formulário|
|9. Seleciona a opção de registrar|
||10. Solicitar confirmação
|11. Confirmar ação|
||12. Registrar a saída dos materiais 

f) **Cenário alternativo - Gestor não confirmou a ação de registro**:
| Ações do ator | Resposta do Sistema
| :----------- | :-------------:|
|1.Selecionar a opção de registrar saída de materiais|
||2.Apresentar formulário para preencher quais materiais foram retirados
|3. Preencher o formulário|
|4.Seleciona a opção de registrar|
||5.Solicita confirmação
|6.Recusa a confirmação|
||7.Solicita se realmente deseja cancelar o registro
|8. Confirma ação|
||9.Retorna ao menu principal

<h3><a name="entrada">3.6 Identificação de caso de uso - <b>CDU006</b> - Registrar entrada de materiais</a></h3>

a) **Ator principal**: Gestor geral

b) **Resumo**: Este caso detalha passo a passo como o gestor irá registrar a entrada de materiais dentro do sistema do laboratório de robótica

c) **Pré-condições**: Gestor deseja realizar a entrada de um material recebido

d) **Cenário principal -  Gestor registra a entrada de material**:

| Ações do ator | Resposta do Sistema
| :----------- | :-------------:|
|1.Selecionar a opção de registro de materiais|
||2.Apresentar formulário para preenchimento dos materiais a serem registrados
|3.Preencher formulário|
|4.Seleciona a opção de registrar material|
||5. Solicitar confirmação
|6. Confirmar ação|
||7. Registra a entrada de materiais no sistema

e) **Cenário alternativo - Gestor não preenche formulário**:
| Ações do ator | Resposta do Sistema
| :----------- | :-------------:|
|1.Selecionar a opção de registro de materiais|
||2.Apresentar formulário para preenchimento dos materiais a serem registrados
|3. Não preenche formulário|
|4.Seleciona opção de registrar material|
||5.Verifica se o relatório está em branco
||6.Informa que o formulário deve ser preenchido
||7.Apresenta formulário de registro
|8. Preenche o formulário
|9.Seleciona opção de registrar material
||10.Verifica se o relatório está em branco
||11.Solicita confirmação
|12. Confirmar ação|
||13.Registra a entrada de materiais no sistema

f) **Cenário alternativo - Gestor deseja cancelar o registro**:

| Ações do ator | Resposta do Sistema
| :----------- | :-------------:|
|1.Selecionar a opção de registro de materiais|
||2.Apresentar formulário para preenchimento dos materiais a serem registrados
|3.Preencher formulário|
|4.Seleciona a opção de registrar material|
||5.Solicitar confirmação
|6. Cancela a confirmação de registro|
||7. Retorna ao menu principal


<h3><a name="aluno">3.7 Identificação de caso de uso - <b>CDU007</b> - Aluno cadastra demandas</a></h3>

a) **Ator principal**: Aluno

b) **Resumo**: Este caso detalha como o aluno irá cadastrar demandas dentro do sistema quando ele retirar algum material do laboratório.

c)**Pré-condições**: Aluno deseja registrar uma demanda no sistema

d) **Cenário Principal - Aluno deseja registrar demanda**:
| Ações do ator | Resposta do Sistema
| :----------- | :-------------:|
|1.Seleciona a opção de Registrar demandas|
||2.Apresenta formulário de registro
|3.Preencher o formulário|
|4.Selecionar opção de registrar demanda|
||5.Solicita confirmação
|6.Confirmar ação|
||7.Demanda registrada com sucesso

e) **Cenário alternativo - Aluno não preenche o formulário**:

| Ações do ator | Resposta do Sistema
| :----------- | :-------------:|
|1.Seleciona a opção de Registrar demandas|
||2.Apresenta formulário de registro
|3.Não preenche o formulário|
|4.Selecionar opção de registrar demanda|
||5.Verifica se o relatório não está em branco
||6.Informa que o formulário deve ser preenchido
||7.Apresenta formulário de registro de demandas
|8. Preenche o formulário|
|9.Seleciona opção de registrar demanda|
||10.Solicita confirmação
|11.Confirmar ação|
||12.Demanda registrada com sucesso

f) **Cenário alternativo - Aluno cancela o registro da demanda**:
| Ações do ator | Resposta do Sistema
| :----------- | :-------------:|
|1.Seleciona a opção de Registrar demandas|
||2.Apresenta formulário de registro
|3.Preencher o formulário|
|4.Selecionar opção de registrar demanda|
||5.Solicitar confirmação
|6.Cancela a confirmação|
||7. Retorna ao menu principal