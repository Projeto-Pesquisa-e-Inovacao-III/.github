# CSF

Este projeto visa a digitalização completa da gestão de alunos, eliminando a dependência de métodos analógicos. O sistema centraliza o controle de disponibilidade, agendamentos e transações financeiras.

## Arquitetura do Projeto

O sistema é composto por três componentes principais:

### 1. Api-system
Responsável pela lógica de negócio principal do domínio.
* **Tecnologias:** Java 21, Spring Boot.
* **Responsabilidades:** Autenticação (Login), gerenciamento de perfil, controle de disponibilidade e gestão de agendamentos.
* **Persistência:** MySQL.

### 2. Api-pag
Microserviço dedicado ao processamento financeiro.
* **Tecnologias:** Java 21, Spring Boot.
* **Responsabilidades:** Processamento de pagamentos, controle de pacotes de aulas e integração com gateways de pagamento.
* **Persistência:** MySQL

### 3. React-app
Interface de usuário para o Personal Trainer.
* **Tecnologias:** React, TypeScript.
* **Responsabilidades:** Consumo da API via REST, visualização de agenda, gestão de alunos e dashboards financeiros.
