
# <h1 align="center"> Trabalho Final - 43SCJ - DEVOPS</h1>

# Objetivo do projeto

Criar um Pipeline para build e deploy de uma aplicação usando Jenkins. Com front end.

# Front End

Desenvolvimento de uma solução para Controle Financeiro. Calculando seu saldo conforme suas receitas e despesas. Foi feito uma API REST e um Front-End. Com persistência local realizada em arquivo JSON e gestão de dependências usando o NPM.

> :construction: Projeto Concluído
  
## ✔️ Executando o projeto Front End

     1. Via terminal pelo Visual Studio Code acessar a pasta webapi do projeto com o comando: cd .\webapi\ 

     2. No terminal executar os seguintes comandos. (Instalar o Node JS e configurar a variável de ambiente 
           para os comando abaixo funcionar):

            - npm install

            - npm install nodemon 

            - npm run start 

     3. Instalar a extensão Life Server no Visual Studio Code. 

     4. Após instalar o Life Server clicar na opção Go Live na parte inferior da tela, conforme print abaixo: 
  
 <img src="https://github.com/victordias25/trabalho-fiap-webservices/blob/main/images/1.PNG">
 
 
 ## ✔️ Como utilizar a ferramenta de Controle Financeiro  

       1. Após clicar na opção Go Live, como mencionado acima. Acessar a ferramenta de Controle Financeiro utilizando 
             a seguinte URL: http://localhost:5500/

       2. Print da tela inicial:

<img src="https://github.com/victordias25/trabalho-fiap-webservices/blob/main/images/2.PNG">

       3. Clicando na opção: “Adicionar Transação” a seguinte tela é aberta:

<img src="https://github.com/victordias25/trabalho-fiap-webservices/blob/main/images/3.PNG">

       4. Após fazer seus lançamentos de Receita e Despesa o Saldo é Calculado:

<img src="https://github.com/victordias25/trabalho-fiap-webservices/blob/main/images/4.PNG">

## ✔️ Executando Jenkins

    1.  Dentro do diretório jenkins existe um arquivo .bat com as configurações do jenkins para subir.
    2.  Dentro do diretório baixar o arquivo .war no site do Jenkins. Link: https://get.jenkins.io/war-stable/2.387.1/
    3.  Como o arquivo é grande não deixei dentro do diretório.
    4.  Com o arquivo .war baixado, acesse o diretório com um terminal de sua preferencia e de o seguinte comando: startJenkins.bat
    5.  Após um tempo o Jenkins ira subir. Use o link para acessar: http://localhost:8080/
    6.  A senha para acessar o Jenkins pela primeira vez estará no prompt
    7.  Você também pode subir o Jenkins usando uma imagem Docker.
    8.  Em seguida instale todos os Plugins e configure o Jenkins.
    9.  Não esqueça de instalar a extensão do Node JS
    10. Configure um Job/ Pipilene no Jenkins usando o seguinte projeto do Git: https://github.com/victordias25/trabalho-devops.git
    11. Como o projeto é público não precisa de credenciais.
    12. Você também pode fazer um fork do projeto para seu Git.
    13. Após a configuração acima execute o Job.
    14. E pronto as pipelines serão executadas.
    
## ✔️ Pipelines

   - ``Build``
   - ``Teste``
   - ``Deliver for development``
   - ``Deploy for production``

## ✔️ Tecnologias utilizadas

- ``Visual Studio Code``
- ``JSON``
- ``HTLM, CSS, JS``
- ``Node.js``
- ``NPM``
- ``Jenkins``
- ``Docker``

## ✔️ Autores

- ``Ali Tannouri Neto``
- ``Matheus Ciribel``
- ``Pedro Henrique Rossi``
- ``Victor Alves Bugueno``
- ``Victor Augusto Pereira Dias Nicola``
