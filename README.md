# Estudae

Projeto que busca ajudar estudantes carentes a conseguir acesso à reforços escolares e a doações de materiais escolares.

## Problema abordado e justificativa

Muitos estudantes de escolas públicas de bairros periféricos têm dificuldade para contratar professores e/ou mentores para fazer um reforço escolar adequado e também tem dificuldade de conseguir materiais de melhor qualidade que custam caro. Nessa situação, muitos estudantes acabam por ir mal na escola e acabam deixando de lado os estudos, por não conseguir compreender os assuntos das matérias e por não conseguir materiais adequados para estudar.

## Objetivos do sistema

O sistema tem como objetivo principal facilitar o acesso dos alunos aos professores de reforço escolar e à voluntários que têm interesse em doar materiais de estudo que não utilizam mais.

## Visão geral da arquitetura

A arquitetura segue um modelo monolítico, que inicialmente resolve bem a questão de cliente-servidor. Caso seja necessário escalar o sistema, poderia ser modificado para um modelo de microsserviços.

Segue o diagrama da arquitetura geral do sistema:

![Diagrama de arquitetura do sistema](docs/architecture/Architecture_Estudae.jpg)

## Tecnologias propostas

- **Front-end:** ReactJS com TS e Vite;
- **Mobile:** React Native com TS;
- **Back-end:** Node.js + Express (APIs RESTfull);
- **Banco de Dados:** Postgres;
- **Autenticação:** Auth simples com bcrypt para senhas.
- **Deploy:**
	- **Front-end:** Vercel;
	- **Mobile:** Play Store
	- **Back-end:** Render;
	- **Database:** Postgres no Render;

## Cronograma Temporário da Etapa 2

> O cronograma é temporário pois a data de entrega ainda não foi definida

| Datas | Tarefas |
|-------|---------|
| **06/10/2025** | Alinhamento dos protótipos e apontamento de melhorias |
| **20/10/2025** | Iniciar o desenvolvimento da API e do front-end |
| **03/11/2025** | Realizar integração cliente-servidor |
| **17/11/2025** | Realizar testes unitários |
| **01/12/2025** | Fazer deploy das aplicações e do banco de dados |
| **15/12/2025** | Fazer testes automatizados |

## Integrantes e papéis

| Nome | Matrícula | Papel |
|------|-----------|-------|
| **Abrahão Levy Barbosa de Lavor** | 2323796 | Product Owner (PO) |
| **Carlos Filipe Madeira de Souza** | 2317449 | Desenvolvedor back-end |
| **Dayon Oliveira de Souza** | 2425030 | Desenvolvedor fullstack |
| **Fernando Luiz Silva de Lima** | 2326203 | QA Engineer |
| **Thiago de Vasconcelos Sousa** | 2415581 | Arquiteto de Software |
| **Sabrina dos Santos Alves** | 2326657 | DevOps Engineer |
