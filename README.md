![Azure](https://img.shields.io/badge/Microsoft-Azure-blue)
![GitHub](https://img.shields.io/badge/Documentação-GitHub-black)
![Status](https://img.shields.io/badge/Status-Concluído-brightgreen)
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

### 3. Escolha do Serviço de Banco de Dados

Para o laboratório, o foco foi a configuração de uma instância de banco de dados no Azure.

Entre as opções disponíveis, é possível encontrar:

Banco de Dados SQL do Azure;
Instância Gerenciada de SQL do Azure;
SQL Server em Máquinas Virtuais.

Cada opção atende a um tipo de necessidade. Para projetos mais simples, o Banco de Dados SQL pode ser suficiente. Para ambientes com maior compatibilidade com SQL Server tradicional, a Instância Gerenciada pode ser mais adequada.

### 4. Configuração Básica da Instância

Durante a criação da instância, alguns campos importantes precisam ser configurados:

Assinatura do Azure;
Grupo de recursos;
Nome da instância;
Região;
Método de autenticação;
Usuário administrador;
Senha;
Configurações de computação e armazenamento.

Essas informações definem como o recurso será criado e acessado.

### 5. Configuração de Rede

A configuração de rede é uma etapa importante, pois define como a instância poderá ser acessada.

Alguns pontos observados:

Rede virtual;
Sub-rede;
Regras de firewall;
Permissões de acesso;
Segurança da conexão.

Em ambientes reais, essa etapa deve ser feita com bastante cuidado para evitar exposição indevida do banco de dados.

### 6. Revisão e Criação do Recurso

Antes de criar a instância, o Azure apresenta uma tela de revisão com todas as configurações escolhidas.

Nessa etapa, é importante verificar:

Nome do recurso;
Região;
Custos estimados;
Configurações de segurança;
Configurações de rede;
Tipo de serviço selecionado.

Após a validação, o recurso pode ser criado.

### 7. Monitoramento da Implantação

Após iniciar a criação do recurso, o Azure exibe o andamento da implantação.

Dependendo do tipo de banco de dados escolhido, a criação pode levar alguns minutos ou até mais tempo em serviços mais robustos, como uma Instância Gerenciada de SQL.

Boas Práticas Observadas

Durante o laboratório, algumas boas práticas foram identificadas:

Utilizar nomes claros para os recursos;
Criar grupos de recursos separados por projeto;
Escolher a região mais adequada para o uso;
Verificar custos antes de criar recursos;
Configurar regras de firewall com cuidado;
Evitar deixar serviços ativos sem necessidade;
Documentar cada etapa do processo;
Excluir recursos após os testes para evitar cobranças.
Dicas Importantes
Atenção aos Custos

Antes de criar qualquer recurso no Azure, é importante verificar o custo estimado. Alguns serviços podem gerar cobranças mesmo quando não estão sendo utilizados diretamente.

### Organização dos Recursos

Usar uma boa nomenclatura facilita muito o gerenciamento dos serviços no portal.

## Exemplo:

rg-dio-lab-azure-sql
sql-dio-lab-db
vnet-dio-lab
Segurança

Nunca compartilhe senhas, strings de conexão ou dados sensíveis em repositórios públicos.

Caso precise documentar exemplos, utilize valores fictícios.

## Exemplo:

Server=tcp:meu-servidor.database.windows.net;
User ID=usuario_exemplo;
Password=senha_exemplo;
Limpeza do Ambiente

Após finalizar o laboratório, é recomendado excluir os recursos criados caso eles não sejam mais necessários. Isso ajuda a evitar custos indesejados.

Possíveis Prints para Adicionar

Caso queira complementar o repositório, é possível criar uma pasta chamada /images e adicionar capturas de tela como:

Tela inicial do Portal Azure;
Criação do grupo de recursos;
Tela de configuração do banco de dados;
Tela de revisão e criação;
Implantação concluída;
Visão geral do recurso criado.

### Aprendizados Finais

Este laboratório foi importante para compreender, na prática, como funciona a criação de uma instância de banco de dados dentro da plataforma Microsoft Azure.

Além da parte técnica, o desafio também reforçou a importância da documentação. Saber explicar o que foi feito, quais decisões foram tomadas e quais cuidados são necessários é uma habilidade essencial para qualquer profissional de tecnologia.

### Com esse projeto, foi possível praticar:

Uso do Portal Azure;
Criação e organização de recursos;
Conceitos de banco de dados em nuvem;
Boas práticas de segurança;
Documentação técnica com Markdown;
Publicação de conteúdo técnico no GitHub.
Referências
Microsoft Learn - Azure SQL Managed Instance
Microsoft Learn - Criar Instância Gerenciada de SQL do Azure
GitHub Docs - Sintaxe básica de escrita e formatação
Documentação Oficial da Microsoft Azure
