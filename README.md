# Sistema-em-camadas-Clinica-Odontologica
O Sistema de Gestão Odontológica é uma aplicação desenvolvida para auxiliar o controle básico das atividades de uma clínica odontológica.

Sistema de Gestão Odontológica
Descrição Geral do Sistema

Este projeto consiste no desenvolvimento de um Sistema de Gestão para Clínica Odontológica, elaborado como atividade acadêmica no curso de Análise e Desenvolvimento de Sistemas. O sistema tem como objetivo apoiar o controle operacional de uma clínica odontológica por meio do gerenciamento de agendamentos, serviços e pagamentos, além da disponibilização de um painel de visualização diária dos atendimentos.

A aplicação foi desenvolvida utilizando arquitetura em camadas, promovendo a separação de responsabilidades entre frontend e backend, bem como entre as camadas internas do servidor, proporcionando melhor organização, manutenção e compreensão do código.

Requisitos Funcionais
Os requisitos funcionais implementados no sistema são:
Permitir o cadastro de agendamentos de pacientes;
Registrar informações como nome, telefone, data, horário, serviço e forma de pagamento;
Armazenar os agendamentos no backend;
Exibir na tela inicial os pacientes agendados para o dia atual;
Listar os serviços odontológicos oferecidos pela clínica;
Listar pagamentos realizados, pendentes e atrasados;
Permitir a filtragem de pagamentos por status;
Disponibilizar horários livres para novos agendamentos.

Requisitos Não Funcionais
Os requisitos não funcionais do sistema incluem:
Execução do sistema em ambiente local;
Utilização do Node.js como plataforma de execução do backend;
Implementação de uma API REST utilizando Express.js;
Comunicação entre frontend e backend via protocolo HTTP;
Persistência de dados realizada por meio de arquivos JSON;
Organização do código seguindo arquitetura em camadas;
Código modularizado e de fácil manutenção;
Compatibilidade com navegadores modernos.

Arquitetura do Sistema
O sistema foi desenvolvido seguindo o modelo de arquitetura em camadas, sendo composto pelas seguintes partes:

Frontend: responsável pela interface com o usuário, desenvolvido em HTML, CSS e JavaScript;

Backend: responsável pelo processamento das regras de negócio e persistência dos dados;

Rotas: responsáveis por definir os endpoints da API;

Controllers: responsáveis pela lógica da aplicação;

Models: responsáveis pela leitura, escrita e manipulação dos dados;

Database: arquivos JSON utilizados como forma de persistência.

A comunicação entre frontend e backend ocorre por meio de requisições HTTP utilizando a função fetch.

Justificativa da Adoção da Arquitetura em Camadas

A adoção da arquitetura em camadas foi motivada pela necessidade de organizar o sistema de forma clara e estruturada, garantindo separação de responsabilidades e redução do acoplamento entre os módulos.

Essa arquitetura facilita a manutenção, a evolução do sistema e o entendimento do fluxo de dados, além de seguir boas práticas de engenharia de software amplamente utilizadas no mercado e abordadas no curso de Análise e Desenvolvimento de Sistemas.

Diagrama Simples da Arquitetura
A arquitetura do sistema pode ser representada de forma simplificada da seguinte maneira:

Frontend (HTML, CSS, JavaScript)
            |
            | Requisições HTTP (fetch)
            v
Backend (Node.js / Express)
            |
            |-- Rotas
            |-- Controllers
            |-- Models
            |
        Arquivos JSON (Database)


O frontend realiza requisições HTTP para o backend, que processa os dados por meio das camadas internas e acessa os arquivos JSON para persistência das informações.

Tecnologias Utilizadas
As tecnologias utilizadas no desenvolvimento do sistema são:
HTML5
CSS3
JavaScript
Node.js
Express.js
JSON
Git
GitHub
Estrutura de Pastas

A estrutura de pastas do projeto está organizada conforme apresentado a seguir:

clinica-odontologica/
├── backend/
│   ├── server.js
│   ├── package.json
│   └── src/
│       ├── app.js
│       ├── routes/
│       │   ├── agendamentoRoutes.js
│       │   ├── dashboardRoutes.js
│       │   ├── pagamentoRoutes.js
│       │   └── servicoRoutes.js
│       ├── controllers/
│       │   ├── agendamentoController.js
│       │   ├── dashboardController.js
│       │   ├── pagamentoController.js
│       │   └── servicoController.js
│       ├── models/
│       │   ├── agendamentoModel.js
│       │   ├── pagamentoModel.js
│       │   └── servicoModel.js
│       └── database/
│           ├── agendamentos.json
│           ├── pagamentos.json
│           └── servicos.json
└── frontend/
    ├── index.html
    ├── agenda.html
    ├── servicos.html
    └── pagamentos.html

Instruções para Execução do Projeto

Para executar o projeto localmente, é necessário seguir os passos abaixo:

Instalar o Node.js no computador;

Clonar o repositório do projeto;

Acessar a pasta backend;

Instalar as dependências do projeto executando o comando:

npm install


Iniciar o servidor backend executando:

npm start


Verificar se o backend está em execução na porta 3001;

Abrir os arquivos HTML localizados na pasta frontend em um navegador;

Utilizar o sistema conforme as funcionalidades disponíveis.

Identificação dos Autores

Nome: Letícia Justino Maciel.

Curso: Análise e Desenvolvimento de Sistemas.

Instituição de Ensino: IFCE Campus Boa Viagem.

Ano: 2026

Observações Finais

Este sistema foi desenvolvido com finalidade acadêmica, visando a aplicação prática dos conceitos de arquitetura em camadas, desenvolvimento backend com Node.js e integração entre frontend e backend por meio de uma API REST.
