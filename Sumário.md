# Sumário

1. [Introdução](#intro)<br>
    - 1.1 [Propósito](#prop)
    - 1.2 [Escopo](#escop)
    - 1.3 [Definições, Acrônimos e Abreviações](#def)
    - 1.4 [Referências]()
    - 1.5 [Visão Geral]()
2. [Posicionamento](#position)
    - 2.1 [Oportunidade de negócio]()
    - 2.2 [Descrição do Problema]()
    - 2.3 [Instrução de Posição do Produto]()
3. [Descrições da parte interessada e dos Usuários]()
    - 3.1 [Resumo dos Usuários]()
    - 3.2 [Perfis dos Usuários]()
4. [Visão Geral do Produto]()
    - 4.1 [Configurações do Produto]()


### <a name="intro">1. Introdução</a>

#### <a name="prop">1.1 Propósito</a>
 O propósito deste documento é expor as necessidades e funcionalidades gerais do sistema de injeção de insulina afim de estabelecer uma visão ampla de modo a deixar claro sua proposta, características e utilidade.

#### <a name="escop">1.2 Escopo</a>

 São tratados nesse documento os pontos necessários para a elaboração do sistema de injetor de insulina que tem como finalidade suprir a necessidade e  gerenciamento das doses de insulina para usuários que tem diabetes.

#### <a name="def">1.3 Definições, Acrônimos e Abreviações</a>
- Profissionais de saúde - A quem compete configurar o equipamento e realizar manutenções, além do acompanhamento do paciente.
 
 #### 1.4 Referências:
 BORGES, felipe; Guilherme;RODRIGUES, natália;Mateus;KISHIMA, lucas. Projeto Receita Mais: Documento de Visão. Disponível em: https://github.com/fga-eps-mds/2017.2-Receita-Mais/wiki/Documento-de-Vis%C3%A3o . Acesso em 24 jul. 2020;

 #### 1.5 Visão Geral

 Este documento é dividido em 4 tópicos descrevendo das características do sistema proposto. Sendo dividido em:
 -  **Introdução**: no qual é introduzido os detalhes gerais sobre a visão do projeto;
 - **Posicionamento**: descrevendo o problema e a oportunidade de negócio;
 - **Descrições dos Envolvidos e dos Usuários**: esta seção descreve o perfil das partes interessadas no projeto;
 - **Visão Geral do Produto**: Esta seção fornece uma visualização de alto nível das capacidades do produto.

### <a name="position">2. Posicionamento</a>

#### 2.1 Oportunidade de Negócio

O número de Brasileiros diagnosticados com diabetes cresceu 61,8% nos últimos 10 anos, de acordo com dados do Ministério da Saúde. Isso significa que 8,9% da população sofre com a doença - eram 5,5% em 2006. Para esses pacientes, assegurar que os níveis de glicose no sangue estejam sempre adequados é um grande desafio.

O sistema de injetor de insulina oferecerá que o aparelho seja uma solução para que os pacientes que tenham diabetes, não venham a ter uma hipoglicemia (queda drástica de taxas de açúcar no sangue). Tornando assim a vida desse indivíduo mais satisfatória.
#### 2.2 Descrição do Problema


O problema de   | Paciente ter hipoglicemia
:--------- | :------
**afeta** | a qualidade de vida do paciente
**cujo impacto é** | a perda de consiência, convulsões e, em casos mais graves, ao óbito
**uma boa solução seria** | um equipamento que injetasse a insulina no paciente periodicamente

#### 2.3 Instrução de Posição do Produto

Para | profissionais de saúde e pacientes
:---- | :----
**Que** | necessitam de uma solução que auxilie no controle de inserção de insulina.
**Onde controle de inserção de Insulina** | é um sistema
**Que** | faz o gerenciamento de doses de insulina automaticamente conforme configurado pela o profissional de saúde

### 3. Descrições da parte interessada e dos Usuários

#### 3.1 Resumo dos Usuários

| Nome        | Descrição           | 
| ------------- |:-------------:| 
| Paciente      | Pessoas que buscam atendimento médico | 
| Médicos      | Todos os profissionais de saúde que utilizam o sistema      |   

#### 3.2 Perfis dos Usuários

##### 3.2.1 Paciente

| Representante        | Paciente     
| ------------- |:-------------: 
| Descrição      | Pessoas que buscam atendimento médico  
| Tipo      |       Usuário que tem interesse em obter atendimento
| Responsabilidade | -
| Critérios de Sucesso | Inserção automatizada de insulina no corpo para evitar hipoglicemia funcionando durante o período de 30 dias, sendo que faltando 5 dias para o fim do prazo o sistema emite um alarme.
| Envolvimento | Alto
| Problemas/Comentários | Possuem faixas etárias diferentes, pacientes de diabete tipo 1 pode vivenciar, a cada ano, de 30 a 50 episódios de hipoglicemia

##### 3.2.2 Médico

| Representante        | Médico     
| ------------- |:-------------: 
| Descrição      | Formados em médicina, com treinamento para utilização correta do produto.  
| Tipo      | Formados em medicina.
| Responsabilidade | Configurar o sistema para que o paciente utilize de forma correta.
| Critérios de Sucesso | Gerenciar a configuração sempre que requisitado e o sistema funciona por 30 dias, sendo que faltando 5 dias para o fim do prazo o sistema emite alarme para paciente e médico.
| Envolvimento | Alto
| Problemas/Comentários | A utilização não deve ser complexa e eles podem não estarem familiarizados com a utilização sendo necessário um treinamento prévio.

### 4. Visão Geral do Produto

O sistema de inserção de insulina irá automatizar as dosagens de insulina no paciente. O profissional de saúde será responsável por configurar o sistema, sendo que apenas uma das formas de configuração funciona por vez. O sistema funciona durante o período de 30 dias, sendo que quando falta 5 dias para o término do prazo ele emite um alarme para o paciente e o respectivo profissional da saúde que acompanha o caso daquele individuo.

#### 4.1 Configurações do produto:

| Tipo de configuração | Descrição
:----: | :----:
Configuração 01: | Injetar automaticamente 5ml de insulina a cada 2 horas
| Configuração 02: | Configuração personalizada de inserção de insulina, sendo possível definir a quantidade a ser inserida e o tempo entre as inserções
| Configuração 03: | Configuração baseada em análise de sangue onde indentifica a quantidade de glicemia e baseado nesta quantidade, ele injeta a insulina necessária, sendo preciso configurar o tempo entre as checagens de glicemia.








