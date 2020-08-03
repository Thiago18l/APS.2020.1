# Sumário

1. [Introdução](#intro)
    - 1.1 [Propósito](#prop)
    - 1.2 [Escopo](#escopo)
    - 1.3 [Definições, Acrônimos e Abreviações](#def)
    - 1.4 [Referências](#ref)
    - 1.5 [Visão Geral](#vision)
2. [Posicionamento](#position)        
    - 2.1 [Oportunidade de negócio](#oportunity)
    - 2.2 [Descrição do Problema](#des)
3. [Descrições da parte interessada e dos Usuários](#desc)
    - 3.1 [Resumo dos Usuários](#resu)
    - 3.2 [Perfis dos Usuários](#perf)
4. [Visão Geral do Produto](#visiong)
    - 4.1 [Perspectiva do Produto](#perspectiva)
    - 4.2 [Resumo dos Recursos](#config)
    - 4.3 [Suposições](#sup)
5. [Restrições](#prog)
    - 5.1 [Restrições de Design](#design)
    - 5.2 [Restrições de implementação](#imple)
    - 5.3 [Restrições de Segurança](#seguranca)
    - 5.4 [Restrições de Uso](#uso)




## <a name="intro">1. Introdução</a>
#### <a name="prop">1.1 Propósito</a>
A finalidade deste documento é informativa, já que irá coletar, analisar e definir as necessidades e as medidas que auxiliam no gerenciamento do laboratório de robótica. Com isso, irá beneficiar todos os envolvidos e abranger todas as perspectivas atingi eis do Sistema, a qual ira o controlar,armazenar e processar as funcionalidades e requisitos ao acesso às informações, garantindo assim um aumento na produtividade, eficiência e segurança do sistema.

#### <a name="escopo">1.2 Escopo</a>

O escopo deste documento se limita a fornecer a todos os envolvidos uma descrição compreensível das funcionalidades que serão atendidas no projeto de software. Quando necessário este documento pode ser atualizado durante todo o ciclo de desenvolvimento da solução.


#### <a name="def">1.3 Definições, Acrônimos e Abreviações</a>

- Profissionais de educação: A quem compete realizar os cadastros no sistema e gerar relatórios das entradas e saídas de recursos sempre que requisitado.
- Alunos: Usuários do laboratório que geram demandas ao sistema.
- SO: Sistema Operancional. ex: Windows, Linux, MacOS


 #### <a name="ref">1.4 Referências:</a>

 BORGES, felipe; Guilherme;RODRIGUES, natália;Mateus;KISHIMA, lucas. Projeto Receita Mais: Documento de Visão. Disponível em: https://github.com/fga-eps-mds/2017.2-Receita-Mais/wiki/Documento-de-Vis%C3%A3o . Acesso em 31 jul. 2020;

BIDIN, simonica. A robótica Educacional: Uma experiência interdisciplinar de aprendizagem no Ensino da Física. Disponível em: https://administradores.com.br/artigos/a-rob%C3%B3tica-educacional. Acesso em 1 ago. 2020;
  #### <a name="vision">1.5 Visão Geral</a>
  
 Este documento é dividido em 5 tópicos descrevendo das características do sistema proposto. Sendo dividido em:
 -  **Introdução**: no qual é introduzido os detalhes gerais sobre a visão do projeto;
 - **Posicionamento**: descrevendo o problema e a oportunidade de negócio;
 - **Descrições dos Envolvidos e dos Usuários**: esta seção descreve o perfil das partes interessadas no projeto;
 - **Visão Geral do Produto**: Esta seção fornece uma visualização das capacidades do produto.
 - **Restrições**: Esta seção fornece dados técnicos sobre o sistema.

 ### <a name="position">2. Posicionamento</a>
 #### <a name="oportunity">2.1 Oportunidade de Negócio</a>
 Atualmente não existe nenhum sistema de controle para a administração do laboratório de robótica, sendo assim, uma oportunidade de negócio bastante ampla, para obter um controle de quem obteve algum material do laboratório.

 Dessa forma, a concepção de um sistema que permita o gerenciamento do laboratório otimizará a organização e produtividade do mesmo. O **EDUROBOTICA** oferecerá um controle inteligente e transparentes dos dados, para caso o gestor necessite de relatórios e verificações de controle, o sistema irá conceder todos os dados necessários de forma simples e concisa, facilitando assim o gerenciamento do laboratório de robótica.

#### <a name="des">2.2 Descrição do Problema</a>

O problema de   | Gerenciamento de recursos
:--------- | :------
**que afeta** | gestores e colaboradores 
**cujo impacto é** | a perda de consistência dos dados, transparência do que é obtido praticamente não existe e a falta de controle do que entra e saí do laboratório.
**uma boa solução seria** | um sistema que organize e crie relatórios utilizando os dados obtidos de forma prática e simples para a melhor organização e controle dos recursos.

### <a name="desc">3. Descrições da parte interessada e dos Usuários</a>
#### <a name="resu">3.1 Resumo dos Usuários</a>

| Nome        | Descrição           | 
| ------------- |:-------------:| 
| Gestor Geral      | São os profissionais de educação que utilizam o sistema, além de pessoas que podem ser responsáveis por gerenciar todos os cadastros e relatórios do sistema | 
| Alunos      | São os colaboradores que utilizam de toda a estrutura fornecida pelo laboratório.      |  


#### <a name="perf">3.2 Perfis dos Usuários</a>

##### 3.2.1 Gestor Geral

| Representante        | Gestor Geral     
| ------------- |:-------------: 
| Descrição      | Profissionais de educação que buscam melhor controle dos materiais do laboratório.
| Tipo      |       Formados em Áreas Tecnologicas com foco em educação ou afins.
| Responsabilidade | Cadastra Assuntos e demandas, gera relatórios, Presta atendimento de demandas e registra entrada e saída de materiais.
| Envolvimento | Alto
| Problemas/Comentários | Pode ser necessário o treinamento do profissional, cujo objetivo é o controle dos dados dos materiais utilizados no laboratório de robótica, além da entrada e saída de recursos.

##### 3.2.1 Alunos

| Representante        | Alunos   
| ------------- |:-------------: 
| Descrição      | Pessoa responsável por abrir demandas no sistema
| Tipo      |      Estudante 
| Responsabilidade | Abre demandas no sistema quando utiliza algum material do laboratório e avalia o atendimento.
| Envolvimento | Alto
| Problemas/Comentários | O aluno sempre deverá abrir uma nova demanda no sistema sempre que retirar algum material do laboratório para ter um controle desses recursos.

### <a name="visiong">4. Visão Geral do Produto</a>
#### <a name="perspectiva">4.1 Perspectiva do Produto</a>
O **EDUROBOTICA** será desenvolvido para ter um maior controle sobre o patrimônio e para melhorar o serviço do laboratório de robótica. É um sistema  de funcionamento interno, que conterá o cadastro de novas demandas como entrada e saída de kit's e componentes, além de robos já montados ou prontos para montar, cadastro de alunos que utilizam o laboratório e seus recursos, obtendo um maior gerenciamento dos gastos de forma organizada para um maior controle sobre os mesmos.

#### <a name="config">4.2 Resumo dos Recursos</a>

| Recurso       | Benefício   
| ------------- |:-------------: 
| Cadastro de Retirada de Material      | Obter um melhor controle dos recursos que saíem do laboratório
| Permitir o envio de anexos      |      O sistema permitirá que sejam vinculados anexos na demanda. 
| Gerenciamento de relatórios | O sistema permitirá o gerenciamento e busca de relatórios anteriores caso o usuário necessite.
| Lista de recursos em falta | Sistema irá avaliar os níveis de recursos dentro do laboratório, gerando assim uma lista de itens em falta para a reposição dos mesmos.
| Registro de entrada de recursos | Permite que o laboratório tenha o controle da entrada de novos recursos, como, verbas, notas fiscais, data de compras e etc.


#### <a name="sup">4.3 Suposições</a>
- Disponível em todos os SO;
- O sistema utilizará usuário e senha;
- Necessita de pessoas treinadas para o uso do sistema;
- Conterá banco de dados PostgreSQL
- Os relatórios são exportáveis para formatos PDF, para que todos os tipos de documentos sejam salvos corretamente e que possa enviá-los para o e-mail a partir da tela de pré-visualização;
- Supõe-se que nas máquinas que utilizaram o sistema, deve ter navegadores web atualizados para a utilização do mesmo.
### <a name="prog">5. Restrições</a>

#### <a name="design">5.1 Restrições de Design</a>

O design será elegante e simples, pensando ao pormenor, onde apenas o essencial tem lugar à vista.

#### <a name="imple">5.2 Restrições de Implementação</a>

O sistema será desenvolvido utilizando Java no backend da aplicação utilizando o framework Spring Boot e JPA para a persistência de dados como um serviço RESTful. No frontend da aplicação será utilizado a linguagem de programação TypeScript com a biblioteca React, utilizando os principios SOLID e metodologias ágeis de desenvolvimento como o TDD (Test Driven Developement).

#### <a name="seguranca">5.3 Restrições de Segurança</a>

O sigilo dos dados deve ser totalmente respeitado, sendo assim só pessoas responsáveis que teram acesso a relatórios e dados brutos do sistema.

#### <a name="uso">5.4 Restrições de Uso</a>

Para o uso do sistema é necessário que o usuário tenha acesso a um dispositivo conectado à internet e que possua um navegador web compatível com o sistema. Caso o usuário não possua acesso à internet, o sistema deve mostrar uma página de erro.
