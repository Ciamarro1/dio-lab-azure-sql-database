# Configuração de Banco de Dados na Microsoft Azure

## Descrição do Projeto

Este repositório foi criado como parte do desafio da DIO, com o objetivo de documentar o processo de configuração de uma instância de Banco de Dados na plataforma Microsoft Azure.

Durante o laboratório, foram praticados conceitos relacionados à computação em nuvem, criação de recursos no Azure, configuração de serviços de banco de dados e documentação técnica utilizando GitHub.

O objetivo principal deste material é servir como apoio para estudos futuros e como registro da experiência prática adquirida durante o desafio.

---

## Objetivos do Desafio

- Aplicar os conceitos aprendidos em um ambiente prático;
- Compreender o processo de criação de uma instância de banco de dados no Azure;
- Documentar etapas técnicas de forma clara e organizada;
- Utilizar o GitHub como ferramenta de compartilhamento de conhecimento;
- Criar um material de apoio para consultas futuras.

---

## Conceitos Aprendidos

Durante o laboratório, foram reforçados alguns conceitos importantes sobre computação em nuvem e banco de dados como serviço.

### Computação em Nuvem

A computação em nuvem permite utilizar recursos de tecnologia, como servidores, armazenamento, redes e bancos de dados, sem a necessidade de manter uma infraestrutura física própria.

No contexto da Microsoft Azure, esses recursos podem ser criados, configurados, monitorados e escalados diretamente pelo portal da plataforma.

### Banco de Dados como Serviço

Um banco de dados como serviço permite que a infraestrutura, manutenção, disponibilidade e parte da administração sejam gerenciadas pelo provedor de nuvem.

Isso reduz a complexidade operacional e permite que o usuário foque mais na aplicação, nos dados e nas regras de negócio.

### Azure SQL

O Azure SQL é uma solução de banco de dados relacional oferecida pela Microsoft Azure. Ele permite criar bancos de dados gerenciados na nuvem, com recursos de segurança, escalabilidade, backup e alta disponibilidade.

### Instância Gerenciada de SQL do Azure

A Instância Gerenciada de SQL do Azure é uma opção voltada para cenários que precisam de maior compatibilidade com o SQL Server tradicional, mas com os benefícios de um serviço gerenciado na nuvem.

Ela é indicada para empresas ou projetos que desejam migrar bancos de dados existentes para o Azure com menos esforço de adaptação.

---

## Etapas Realizadas no Laboratório

### 1. Acesso ao Portal Azure

O primeiro passo foi acessar o portal da Microsoft Azure, onde é possível visualizar, criar e gerenciar os recursos disponíveis na plataforma.

No portal, é possível pesquisar por serviços como:

- Azure SQL;
- SQL Database;
- SQL Managed Instance;
- Resource Groups;
- Virtual Networks.

---

### 2. Criação de um Grupo de Recursos

O grupo de recursos funciona como um contêiner lógico para organizar os serviços criados dentro do Azure.

Durante a configuração, é importante definir:

- Nome do grupo de recursos;
- Região onde os recursos serão criados;
- Organização dos serviços relacionados ao mesmo projeto.

Exemplo de nome:

```text
rg-dio-lab-azure-sql
