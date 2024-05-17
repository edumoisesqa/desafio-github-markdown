# 
Desafio  da dio para implementar markdown no git hub 


# CATe-QA
Este projeto tem o intuito de formar os QAs qualificados para dentro dos times da Atlas Technologies!



AUTOMATED SOFTWARE TESTING WITH CYPRESS WITH BDD

--Este repositório contem a automação de duas features login e registro de novo usuário 
do desafio CATE - QA

--Toda configuração e realizada através do arquivo cypress.config.ts 
onde foram realizadas modificações para utilizar o BDD com cypress para facilitar a documentação para todos os stakeholder 
Os cenários contemplados estão dentro da pasta scenarios.fature onde descrevo de forma objetiva e simplificada qual teste esta sendo efetuado
 e resultado esperado

No arquivo command.js foi configurado a lib. cypress-file-upload que apoia nos teste de upload de imagem 
Também foi utilizado a lib faker para gerar massas aleatórias, deixando a massa sempre viva e melhor reaproveitamento dos cenários 

Pre-requisitos

"@badeball/cypress-cucumber-preprocessor": "latest",
"@bahmutov/cypress-esbuild-preprocessor": "latest",
"cypress": "latest",
"cypress-file-upload": "^5.0.8",
"faker": "^6.6.6",
"faker-br": "latest",
"typescript": "latest"


Building
[run npm install]

Para iniciar os testes utilize  o seguinte comando
[Run npx cypress open]


Observação: Por algum motivo a VM disponibilizada não estava conseguindo permitir o framework cypress acessar a url http://fm-cate:8080/
após uma forca tarefa da gestão e equipe  foi proposto uma alternativa que era acessar o ip local baseUrl: "http://10.0.52.145:8080"
porem foi necessário recomeçar a automação.
Outro ponto a aplicação não está persistindo os dados, com isso alguns cenários como usuário logado, reenvio de e-mail, ou validar cadastro de um e-mail ja utilizado 
não foi possível automatizar, assim como logout
como temos outras atividades para entregar não vou conseguir direcionar tempo para resolver essas questões de ambiente, acredito que o código feito até o momento mostra o conhecimento sobre padrão de projeto, orientação de projeto, BDD
e cypress.
