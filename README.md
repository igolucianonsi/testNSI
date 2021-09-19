
# Processo seletivo - QA

  

Bem vindo, candidato.

  

Estamos felizes que você esteja participando do processo seletivo para a vaga de QA do Instituto SENAI de Tecnologia em Soluções digitais.

  

A prova utilizará das seguintes tecnologias:

- Linguagem de programação para web

- Docker

- Banco de dados relacional

- GIT

  

Fica à sua escolha quais frameworks e servidor serão utilizados, desde que seja uma aplicação web.

  

O banco de dados relacional deverá ser postgreSQL.

  

Na etapa da entrevista deverá ser apresentado a aplicação em funcionamento.

  

## Instruções para a execução da prova

  

A prova deve ser uma aplicação web. Você pode escolher a tecnologia que achar conveniente (PHP, JAVA, etc...).

  

O Banco utilizado na prova deve ser PostgreSQL.

  

Esse repositório possui apenas esse Readme com as instruções da prova. No entanto, **todo desenvolvimento deve ser commitado nesse repositório** até a data citada no email, enviado por nossa equipe.

  

Commite nesse repositório o script utilizado na criação do banco de dados (se aplicável).

  

Por fim, altere esse arquivo com as instruções de como poderemos testar o seu código (quais libs usar, qual servidor, etc) abaixo.

  

## Será avaliado

- Qualidade do código quanto a:

- Facilidade no entedimento

- Complexidade ciclomática

- Divisão de resposabilidade das classes

- Reutilização de código

- Qualidade quanto a interface:

- Fácil usabilidade

- Acessibilidade

- Feedback ao usuário

- Qualidade quanto aos requisitos:

- Desenvolvimento e funcionamento dos requisitos propostos

  

## Informações extras

  

- Descreva ao final deste documento (Readme.md) o detalhamento de funcionalidades implementadas, sejam elas já descritas na modelagem e / ou extras.

- Detalhar também as funcionalidades que não conseguiu implementar e o motivo.

- Caso tenha adicionado novas libs ou frameworks, descreva quais foram e porque dessa agregação.

  

(Escreva aqui as instruções para que possamos corrigir sua prova, bem como qualquer outra observação sobre a prova que achar pertinente compartilhar)
  
> *Sobre a Prova...*
## Instrução para testes

Utilizo o servidor da Google Cloud para hospedagem da aplicação desenvolvida (Cloud Run), banco de dados também na mesma estrutura de nuvem (Cloud SQL) e pode ser acessada no seguinte link:

	https://php-caecrgswkq-uc.a.run.app

## Funcionalidades do APP
**TELAS:**

>***Home:** Interface inicial da aplicação composta por um cabeçalho contendo um ícone com link para a página principal e logomarca do SENAI. Possui também um menu onde o usuário irá navegar por todo APP, bem como uma mensagem de "bem-vindo" e um painel com resumo de pessoas matriculadas nos cursos.*
>
![alt text](https://raw.githubusercontent.com/CETEC-DIGI/01859-2021-512.748.682-20/dev/telas/tela1.png?token=AVIRZVVPTCFSIBEXRXMSUBTBI6JAS)

>***Pessoa:** Tela onde serão fornecido os dados para ações cadastrais (Inserir/Atualizar/Excluir/Listar) de pessoas. O formulário contém campos (CPF e Data de Nascimento) com máscaras de formatação bem como rotina para validação quanto ao preenchimento dos itens. Foi feito também um bloqueio para exclusão quando a pessoa estiver vinculada a uma matricula.* 
>
![enter image description here](https://raw.githubusercontent.com/CETEC-DIGI/01859-2021-512.748.682-20/dev/telas/tela2.png?token=AVIRZVW7D7FA7EBQVDZYQK3BI6JIY)

>***Curso:** Assim como as funcionalidades básicas da tela de Pessoa a tela Curso possui uma particularidade no item "vagas totais" onde não será permitido editá-lo com valor menor do que a quantidade de matrículas já efetuadas para o mesmo.* 

![enter image description here](https://raw.githubusercontent.com/CETEC-DIGI/01859-2021-512.748.682-20/dev/telas/tela3.png?token=AVIRZVX7P3YNBPDGOPPDQS3BI6KLI)

>***Matrícula:** Nessa área o usuário poderá selecionar a pessoa e o curso de interesse, informar a data da matrícula e assim efetivar a mesma após a verificação de alguns critérios como: a existência de vaga disponíveis no curso, idade mínima do aluno para cursar, se o curso ainda não começou e claro, se o aluno já não foi cadastrado no mesmo curso. Lembrando que essa tela Matrícula possui as mesmas operações básicas das demais quanto ao critério de validação e máscara no campo editável.* 

![enter image description here](https://raw.githubusercontent.com/CETEC-DIGI/01859-2021-512.748.682-20/dev/telas/tela4.png?token=AVIRZVUH25ESCJ4UK2GMSFTBI6LJU)

## Utilizei no desenvolvimento as seguintes ferramentas:

**Framework/Bibliotecas/Plugins/API**
- **Codeigniter 4:** seguro e rápido, minimiza a quantidade de código necessária para execução tarefas rotineiras e com muitos recursos, mas sem deixar o desenvolvimento totalmente dependente apenas dos recursos dele.
- **PHPUnit:** utilizado para realização de testes unitários em PHP.
- **Font Awesome:** reúne vários elemento embutidos utilizados para fontes e ícones com base em CSS e LESS.
- **Bootstrap:** usado para organização e gerência do layout.
- **jQuery:** biblioteca leve, rápida e cheia de recursos para Javascript que facilita a manipulação de eventos, animações, elementos HTML e utilização de Ajax.

- **Masked Input:** plugin que funciona em conjunto com a biblioteca jQuery permite a aplicação de uma máscara de entrada para campos de formulário do tipo input.
- **Validator:** plugin utilizado para validar itens de um formulário e funciona também em conjunto com a biblioteca jQuery.
- **SweetAlert:** API utilizada para estilizar e adicionar funcionalidades às caixas de diálogos em aplicações web.

**Banco de Dados**
- PostgreSQL;
