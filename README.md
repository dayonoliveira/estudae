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

## Integrantes e papéis

Abrahão Levy Barbosa de Lavor: Product Owner;
Carlos Filipe Madeira de Souza: Desenvolvedor back-end;
Dayon Oliveira de Souza: Desenvolvedor full stack;
Fernando Luiz Silva de Lima: QA;
Sabrina dos Santos Alves: Arquiteto de Software;
Thiago de Vasconcelos Sousa: Engenheira de DevOps.