# DanyMed Clinic System

Sistema de gestão clínica desenvolvido com foco em **arquitetura escalável**, **boas práticas de engenharia de software** e preparação para evolução para microserviços.

## Código-fonte

A implementação completa deste projeto está mantida em um repositório privado.
Este repositório público tem como objetivo apresentar a arquitetura, decisões técnicas e evolução do sistema.
Caso tenha interesse em acesso ou detalhes técnicos adicionais, entre em contato.

## Tecnologias

* Java 21
* Spring Boot
* Maven
* PostgreSQL (futuro)
* Docker (futuro)

## Arquitetura

O sistema segue o padrão de **Monolito Modular**, permitindo alta coesão e baixo acoplamento entre os domínios.

Cada módulo representa um contexto de negócio independente, preparado para futura extração como microserviço.

## Estrutura do Projeto

```
clinic-system/
 ├── src/
 │   ├── modules/
 │   │   ├── paciente/          # Gestão de pacientes
 │   │   ├── agenda/            # Agendamentos
 │   │   ├── prontuario/        # Prontuário eletrônico
 │   │   └── notificacao/       # Notificações
 │   │
 │   ├── shared/                # Componentes compartilhados
 │   │   ├── exceptions/
 │   │   ├── utils/
 │   │   └── config/
 │   │
 │   └── main/                  # Classe principal da aplicação
 │
 ├── infra/                     # Infraestrutura
 │   ├── database/
 │   ├── messaging/
 │   └── observability/
 │
 ├── application.yml
 ├── Dockerfile
 ├── pom.xml
 └── README.md
```

## ⚙️ Como executar o projeto

```bash
mvn spring-boot:run
```

## Roadmap

* [x] Estrutura inicial do projeto
* [ ] CRUD de pacientes
* [ ] Módulo de agendamento
* [ ] Autenticação e autorização (JWT)
* [ ] Observabilidade (logs, métricas)
* [ ] Mensageria (event-driven)
* [ ] Dockerização completa

## Conceitos aplicados

* Monolito Modular
* Clean Architecture
* Domain-Driven Design (DDD)
* Separação de responsabilidades
* Preparação para Microserviços

## Autor

Saulo Costa
Senior Software Engineer | Building Scalable Systems | TypeScript, Java, AWS, Microservices

## Licença

Este projeto está sob a licença MIT.
