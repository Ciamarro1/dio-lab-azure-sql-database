# Laboratório: Configuração de Banco de Dados na Microsoft Azure

![Azure](https://img.shields.io/badge/Microsoft-Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![SQL](https://img.shields.io/badge/Azure_SQL-Database-blue?style=for-the-badge)
![GitHub](https://img.shields.io/badge/Documentação-GitHub-181717?style=for-the-badge&logo=github)
![Status](https://img.shields.io/badge/Status-Concluído-brightgreen?style=for-the-badge)

## Sumário

- [Descrição do Projeto](#descrição-do-projeto)
- [Objetivo do Laboratório](#objetivo-do-laboratório)
- [Tecnologias e Ferramentas Utilizadas](#tecnologias-e-ferramentas-utilizadas)
- [Conceitos Trabalhados](#conceitos-trabalhados)
- [Etapas Executadas](#etapas-executadas)
- [Boas Práticas Aplicadas](#boas-práticas-aplicadas)
- [Segurança e Governança](#segurança-e-governança)
- [Custos e Otimização](#custos-e-otimização)
- [Possíveis Erros e Pontos de Atenção](#possíveis-erros-e-pontos-de-atenção)
- [Aprendizados Obtidos](#aprendizados-obtidos)
- [Referências](#referências)

---

## Descrição do Projeto

Este repositório documenta a execução de um laboratório prático voltado à configuração de uma instância de Banco de Dados na plataforma Microsoft Azure.

O objetivo principal foi compreender, de forma prática, como um serviço de banco de dados pode ser criado, configurado, validado e documentado dentro de um ambiente de nuvem.

Além da criação do recurso, este projeto também tem como finalidade registrar os principais conceitos aprendidos durante o laboratório, servindo como material de apoio para estudos futuros, revisões técnicas e futuras implementações em ambientes reais.

---

## Objetivo do Laboratório

O laboratório teve como objetivo praticar o processo de configuração de uma instância de Banco de Dados no Microsoft Azure, explorando conceitos fundamentais de computação em nuvem, banco de dados como serviço, segurança, organização de recursos e documentação técnica.

Os principais objetivos foram:

- Criar e organizar recursos dentro do Microsoft Azure;
- Compreender o funcionamento básico de serviços de banco de dados em nuvem;
- Analisar as principais configurações disponíveis durante a criação de uma instância;
- Documentar o processo técnico de forma clara e estruturada;
- Utilizar o GitHub como ferramenta de versionamento e publicação da documentação;
- Desenvolver uma base de consulta para futuras implementações.

---

## Tecnologias e Ferramentas Utilizadas

Durante o laboratório, foram utilizadas as seguintes tecnologias e ferramentas:

| Ferramenta | Finalidade |
|----------|------------|
| Microsoft Azure | Plataforma de computação em nuvem utilizada para criação dos recursos |
| Azure SQL | Serviço de banco de dados relacional gerenciado |
| Azure Portal | Interface gráfica utilizada para configuração dos recursos |
| Git | Controle de versão do projeto |
| GitHub | Hospedagem do repositório e documentação |
| Markdown | Linguagem de marcação utilizada na criação deste README |

---

## Conceitos Trabalhados

### Computação em Nuvem

Computação em nuvem é um modelo que permite o acesso sob demanda a recursos computacionais, como servidores, redes, armazenamento, bancos de dados e aplicações, sem a necessidade de manter infraestrutura física local.

No contexto deste laboratório, a nuvem foi utilizada para provisionar um serviço de banco de dados gerenciado dentro da plataforma Microsoft Azure.

---

### IaaS, PaaS e SaaS

Durante o estudo, foi possível entender a diferença entre os principais modelos de serviço em nuvem:

| Modelo | Descrição |
|------|-----------|
| IaaS | Infraestrutura como Serviço. O usuário gerencia sistema operacional, aplicações e parte da infraestrutura lógica. |
| PaaS | Plataforma como Serviço. O provedor gerencia a infraestrutura e o usuário foca na aplicação e nos dados. |
| SaaS | Software como Serviço. O usuário consome uma aplicação pronta, sem gerenciar infraestrutura. |

O Azure SQL se encaixa principalmente no modelo PaaS, pois oferece um banco de dados gerenciado, reduzindo a necessidade de administração manual da infraestrutura.

---

### Banco de Dados como Serviço

Banco de Dados como Serviço permite criar, gerenciar e escalar bancos de dados diretamente na nuvem.

Esse modelo oferece vantagens como:

- Menor necessidade de administração de infraestrutura;
- Escalabilidade;
- Alta disponibilidade;
- Backup automatizado;
- Segurança integrada;
- Monitoramento centralizado;
- Redução da complexidade operacional.

---

### Azure SQL

Azure SQL é a família de serviços de banco de dados relacional da Microsoft Azure baseada no mecanismo do SQL Server.

Entre as opções disponíveis, estão:

- Azure SQL Database;
- Azure SQL Managed Instance;
- SQL Server em Máquinas Virtuais.

Cada uma dessas opções atende a diferentes cenários de uso.

---

### Azure SQL Database

O Azure SQL Database é um banco de dados relacional totalmente gerenciado, indicado para aplicações modernas em nuvem.

Ele é recomendado para cenários onde o usuário deseja criar um banco de dados individual com alta disponibilidade, segurança e escalabilidade, sem precisar administrar servidores físicos ou virtuais.

---

### Azure SQL Managed Instance

A Instância Gerenciada de SQL do Azure oferece maior compatibilidade com o SQL Server tradicional.

Ela é indicada principalmente para cenários de migração de bancos de dados locais para a nuvem, mantendo recursos mais próximos de uma instância SQL Server convencional.

---

## Etapas Executadas

### 1. Acesso ao Portal Azure

A primeira etapa consistiu em acessar o portal do Microsoft Azure.

Por meio do portal, é possível criar, configurar, monitorar e excluir recursos de nuvem de forma centralizada.

Endereço do portal: <https://portal.azure.com>

---

### 2. Criação de um Grupo de Recursos

O grupo de recursos foi utilizado para organizar todos os serviços relacionados ao laboratório.

Um grupo de recursos funciona como um contêiner lógico dentro do Azure, permitindo agrupar recursos que pertencem ao mesmo projeto, ambiente ou aplicação.

Exemplo de nomenclatura utilizada:

`rg-dio-lab-azure-sql`

Benefícios do uso de grupos de recursos:

- Organização dos serviços;
- Controle de permissões;
- Facilidade para monitoramento;
- Facilidade para exclusão dos recursos após o laboratório;
- Melhor gestão de custos.

---

### 3. Escolha do Serviço de Banco de Dados

Após a criação do grupo de recursos, foi pesquisado o serviço de banco de dados no Azure Portal.

Foram analisadas opções como:

- Azure SQL Database;
- Azure SQL Managed Instance;
- SQL Server on Azure Virtual Machines.

Para fins de estudo, o foco do laboratório foi compreender a configuração de uma instância de banco de dados no Azure, observando suas opções de provisionamento, autenticação, rede, segurança e custo.

---

### 4. Configuração Básica do Recurso

Durante a configuração inicial, foram definidos os principais parâmetros do serviço.

| Campo | Descrição |
|-----|-----------|
| Subscription | Assinatura do Azure utilizada para cobrança e gerenciamento. |
| Resource Group | Grupo de recursos onde o banco será criado. |
| Database Name | Nome do banco de dados. |
| Server | Servidor lógico associado ao banco. |
| Region | Região geográfica onde o recurso será provisionado. |
| Authentication Method | Método de autenticação utilizado. |
| Admin Login | Usuário administrador do servidor. |
| Password | Senha do usuário administrador. |

Exemplo de nome para banco de dados:

`sqldb-dio-lab`

Exemplo de nome para servidor lógico:

`sqlserver-dio-lab`

---

### 5. Configuração de Autenticação

A autenticação define como os usuários poderão acessar o banco de dados.

Foram observadas opções como:

- Autenticação SQL;
- Autenticação Microsoft Entra ID;
- Autenticação mista, dependendo do cenário.

Para ambientes reais, recomenda-se utilizar mecanismos seguros de autenticação, aplicar o princípio do menor privilégio e evitar o compartilhamento de credenciais administrativas.

---

### 6. Configuração de Rede

A configuração de rede define como o banco de dados poderá ser acessado.

Pontos analisados:

- Acesso público;
- Regras de firewall;
- Redes virtuais;
- Endereços IP permitidos;
- Conectividade privada;
- Segurança da comunicação.

Em cenários produtivos, o ideal é restringir o acesso ao banco de dados apenas a origens confiáveis.

---

### 7. Configuração de Computação e Armazenamento

Durante a criação do recurso, foram avaliadas as opções de desempenho e armazenamento.

Essas configurações impactam diretamente:

- Capacidade de processamento;
- Quantidade de armazenamento disponível;
- Performance do banco;
- Custo do serviço;
- Escalabilidade.

Em um ambiente de laboratório, recomenda-se escolher configurações mínimas ou de baixo custo, apenas para fins de aprendizado.

---

### 8. Revisão das Configurações

Antes da criação do recurso, o Azure apresenta uma tela de revisão.

Nesta etapa, foram conferidos os seguintes itens:

- Nome do recurso;
- Grupo de recursos;
- Região;
- Tipo de serviço;
- Configurações de rede;
- Configurações de autenticação;
- Estimativa de custo;
- Políticas aplicadas.

Essa revisão é importante para evitar erros de configuração e cobranças desnecessárias.

---

### 9. Implantação do Recurso

Após a validação das configurações, foi iniciada a implantação do recurso.

O Azure exibe o status da implantação em tempo real, permitindo acompanhar se o processo foi concluído com sucesso ou se ocorreu alguma falha.

Após a implantação, o recurso fica disponível no grupo de recursos selecionado.

---

### 10. Validação do Recurso Criado

Depois da criação, foi possível acessar a página de visão geral do recurso.

Foram observadas informações como:

- Nome do banco;
- Nome do servidor;
- Status;
- Região;
- Grupo de recursos;
- Configurações de conexão;
- Métricas iniciais;
- Opções de monitoramento.

Essa etapa confirma que o banco de dados foi criado corretamente.

---

## Boas Práticas Aplicadas

Durante o laboratório, foram observadas algumas boas práticas importantes.

### Organização

Utilizar nomes padronizados para os recursos facilita a administração do ambiente.

Exemplos:

- `rg-dio-lab-azure-sql`
- `sqlserver-dio-lab`
- `sqldb-dio-lab`

---

### Separação por Ambiente

Em ambientes reais, recomenda-se separar os recursos por ambiente.

Exemplos:

- `dev`
- `test`
- `homolog`
- `prod`

Essa separação ajuda a evitar alterações indevidas em ambientes produtivos.

---

### Princípio do Menor Privilégio

Usuários e aplicações devem ter apenas as permissões necessárias para executar suas funções.

Evitar o uso constante de usuários administradores reduz riscos de segurança.

---

### Documentação

Documentar o processo é essencial para:

- Reproduzir configurações;
- Compartilhar conhecimento;
- Facilitar manutenção;
- Apoiar troubleshooting;
- Criar histórico técnico do projeto.

---

### Exclusão de Recursos Não Utilizados

Após o laboratório, é recomendado excluir recursos que não serão mais utilizados.

Isso evita cobranças desnecessárias na assinatura Azure.

---

## Segurança e Governança

A segurança é um dos pontos mais importantes ao trabalhar com banco de dados em nuvem.

Algumas práticas recomendadas:

- Não expor o banco de dados publicamente sem necessidade;
- Utilizar regras de firewall restritivas;
- Proteger credenciais de acesso;
- Não publicar senhas ou strings de conexão no GitHub;
- Utilizar autenticação integrada sempre que possível;
- Monitorar tentativas de acesso;
- Aplicar controle de acesso baseado em função;
- Revisar permissões periodicamente.

Exemplo de string de conexão fictícia:

```text
Server=tcp:sqlserver-dio-lab.database.windows.net,1433;
Initial Catalog=sqldb-dio-lab;
Persist Security Info=False;
User ID=usuario_exemplo;
Password=senha_exemplo;
MultipleActiveResultSets=False;
Encrypt=True;
TrustServerCertificate=False;
Connection Timeout=30;
```

> Observação: a string acima é apenas um exemplo fictício. Nunca publique credenciais reais em repositórios públicos.

---

## Custos e Otimização

Durante a criação de recursos no Azure, é importante observar os custos estimados.

Alguns fatores que impactam o custo:

- Região escolhida;
- Tipo de serviço;
- Camada de desempenho;
- Armazenamento provisionado;
- Tempo em que o recurso permanece ativo;
- Backups;
- Tráfego de rede;
- Alta disponibilidade.

Boas práticas para controle de custos:

- Utilizar recursos mínimos em ambiente de estudo;
- Excluir recursos após o uso;
- Monitorar custos pelo Azure Cost Management;
- Configurar alertas de orçamento;
- Evitar recursos superdimensionados;
- Revisar periodicamente os serviços ativos.

---

## Possíveis Erros e Pontos de Atenção

Durante a configuração de um banco de dados no Azure, alguns problemas podem ocorrer.

### Erro de Região

Nem todos os serviços ou configurações estão disponíveis em todas as regiões.

Solução:

- Verificar se o serviço escolhido está disponível na região selecionada;
- Escolher uma região alternativa, se necessário.

---

### Erro de Senha Inválida

O Azure exige senhas com critérios mínimos de complexidade.

Solução:

- Utilizar letras maiúsculas;
- Utilizar letras minúsculas;
- Utilizar números;
- Utilizar caracteres especiais;
- Evitar senhas simples ou previsíveis.

---

### Erro de Firewall

Mesmo com o banco criado, o acesso pode falhar caso o IP do usuário não esteja autorizado.

Solução:

- Configurar as regras de firewall;
- Permitir o IP correto;
- Revisar as configurações de rede.

---

### Custo Acima do Esperado

Recursos mal dimensionados podem gerar custos desnecessários.

Solução:

- Revisar a camada de serviço escolhida;
- Usar configurações mínimas para laboratório;
- Excluir recursos após os testes;
- Monitorar os custos no portal.

---

## Sugestão de Evidências

Caso necessário, a pasta `images` pode ser utilizada para armazenar capturas de tela do laboratório.

Exemplos de evidências:

- `images/01-portal-azure.png`
- `images/02-resource-group.png`
- `images/03-configuracao-banco.png`
- `images/04-revisao-criacao.png`
- `images/05-deploy-concluido.png`
- `images/06-visao-geral-recurso.png`

Exemplo de inserção de imagem no README:

```markdown
![Visão geral do recurso criado](./images/06-visao-geral-recurso.png)
```

---

## Estrutura do Repositório

```text
dio-lab-azure-sql-database/
├── README.md
└── images/
    ├── 01-portal-azure.png
    ├── 02-resource-group.png
    ├── 03-configuracao-banco.png
    ├── 04-revisao-criacao.png
    ├── 05-deploy-concluido.png
    └── 06-visao-geral-recurso.png
```

A pasta `images` é opcional e pode ser utilizada caso sejam adicionadas capturas de tela do processo.

---

## Comandos Git Utilizados

Exemplo de comandos para versionar e enviar o projeto ao GitHub:

```bash
git init
git add .
git commit -m "docs: adiciona documentação do laboratório Azure SQL"
git branch -M main
git remote add origin https://github.com/seu-usuario/dio-lab-azure-sql-database.git
git push -u origin main
```

---

## Aprendizados Obtidos

Com a realização deste laboratório, foi possível compreender melhor o funcionamento da criação de recursos de banco de dados na nuvem utilizando a Microsoft Azure.

Os principais aprendizados foram:

- Como acessar e navegar pelo Portal Azure;
- Como organizar recursos utilizando grupos de recursos;
- Como identificar serviços de banco de dados disponíveis na plataforma;
- Como configurar parâmetros básicos de uma instância de banco de dados;
- Como avaliar opções de autenticação, rede, desempenho e custo;
- Como aplicar boas práticas de segurança;
- Como documentar um processo técnico no GitHub;
- Como estruturar um README profissional para entrega de projeto.

Este laboratório reforçou a importância da documentação técnica como parte do processo de aprendizado e da atuação profissional em tecnologia.

---

## Conclusão

A configuração de uma instância de banco de dados no Microsoft Azure permite entender, na prática, como serviços gerenciados em nuvem são provisionados e administrados.

O uso de banco de dados como serviço reduz a complexidade de infraestrutura e oferece recursos importantes de segurança, disponibilidade, escalabilidade e monitoramento.

Além da prática com Azure, este desafio também contribuiu para o desenvolvimento de habilidades essenciais em documentação técnica, organização de repositórios e compartilhamento de conhecimento por meio do GitHub.

---

## Referências

- [Microsoft Azure - Documentação Oficial](https://learn.microsoft.com/pt-br/azure/)
- [Azure SQL - Documentação Oficial](https://learn.microsoft.com/pt-br/azure/azure-sql/)
- [Criar Instância Gerenciada de SQL do Azure](https://learn.microsoft.com/pt-br/azure/azure-sql/managed-instance/instance-create-quickstart)
- [GitHub Docs](https://docs.github.com/pt)
- [Sintaxe básica de Markdown no GitHub](https://docs.github.com/pt/get-started/writing-on-github)
