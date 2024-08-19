# Diferença entre dados estruturados, semiestruturados e não estruturados
- **Dados Estruturados**: Dados organizados em um formato pré-definido, como tabelas de bancos de dados com colunas e tipos de dados específicos.
- **Dados Semiestruturados**: Dados parcialmente estruturados, como JSON ou XML, que possuem uma organização hierárquica, mas não seguem um esquema rígido.
- **Dados Não Estruturados**: Dados que não possuem uma organização ou estrutura definida, como vídeos, imagens, ou textos livres.

# Compreensão de serviços de dados: Bancos de Dados Relacionais e NoSQL
- **Bancos de Dados Relacionais**: Estruturados em tabelas com chaves primárias e estrangeiras, usando SQL para consultas. Ex.: MySQL, PostgreSQL.
- **Bancos de Dados NoSQL**: Flexíveis em estrutura, usados para dados distribuídos e de grande escala. Ex.: MongoDB, Cassandra.

# Modelos de Dados
- **Normalização**: Processo de organizar os dados para reduzir a redundância e dependência, dividindo-os em várias tabelas relacionadas.
- **Desnormalização**: Combinação de dados normalizados para melhorar o desempenho de leitura, mesmo que isso aumente a redundância.

## Conceitos de Dados Relacionais
- **Conceitos**: Bancos de dados relacionais são organizados em tabelas que representam entidades. As relações entre tabelas são feitas através de chaves primárias (únicas para cada registro) e chaves estrangeiras (que referenciam chaves primárias em outras tabelas).
- **SQL e Operações Comuns**:
  - **SELECT**: Consulta para recuperar dados.
  - **JOIN**: Combina dados de duas ou mais tabelas.
  - **Agregações**: Operações como SUM, COUNT, AVG aplicadas em grupos de dados.
- **Serviços de Banco de Dados Relacionais no Azure**:
  - Azure SQL Database
  - SQL Managed Instance

## Conceitos de Dados Não Relacionais
- **Diferença entre Bancos de Dados NoSQL e Relacionais**: Bancos NoSQL não utilizam esquema fixo e são mais flexíveis, enquanto os relacionais seguem um esquema rígido com tabelas, colunas e tipos de dados definidos.
- **Serviços de Banco de Dados NoSQL no Azure**:
  - Azure Cosmos DB
- **Casos de Uso de Dados Não Relacionais**: Ideal para grandes volumes de dados não estruturados ou semiestruturados, como redes sociais, catálogos de produtos e dados de IoT.

## Conceitos de Análise de Dados
- **Processamento de Dados para Análise**:
  - **ETL** (Extract, Transform, Load): Processo de extração, transformação e carregamento de dados em um sistema de destino.
  - **ELT** (Extract, Load, Transform): Processo em que os dados são carregados no sistema de destino antes de serem transformados.
- **Armazenamento de Dados no Azure**:
  - Azure Data Lake
  - Armazenamento Blob
- **Ferramentas de Análise de Dados no Azure**:
  - Azure Synapse Analytics
  - Power BI

# Azure Synapse Analytics
- **Azure Synapse Analytics**: Serviço de análise integrado que combina big data e análise de dados empresariais. Ele permite o processamento de consultas SQL e a execução de pipelines de dados em grande escala, fornecendo insights em tempo real.

# Blobs
- **Blobs**: São objetos de armazenamento no Azure Blob Storage usados para armazenar grandes quantidades de dados não estruturados, como imagens, vídeos, documentos e backups.

# Instruções SQL
- **Instruções SQL**: Conjunto de comandos usados para gerenciar e consultar bancos de dados relacionais. As principais instruções incluem:
  - **SELECT**: Recupera dados de uma tabela.
  - **INSERT**: Insere novos dados em uma tabela.
  - **UPDATE**: Atualiza dados existentes em uma tabela.
  - **DELETE**: Remove dados de uma tabela.



# Apache Gremlin
- **Apache Gremlin**: Linguagem de consulta usada para trabalhar com bancos de dados de grafos. Ele permite consultas complexas em estruturas de dados de grafos, que são compostas de vértices e arestas.

# Apache Cassandra
- **Apache Cassandra**: Banco de dados NoSQL altamente escalável e distribuído, projetado para lidar com grandes volumes de dados em múltiplos servidores, sem pontos de falha.

# CosmosDB
- **Azure Cosmos DB**: Banco de dados NoSQL distribuído globalmente que oferece suporte a vários modelos de dados (chave-valor, documento, gráfico, etc.). Ele é conhecido por sua baixa latência e alta disponibilidade.

# MongoDB
- **MongoDB**: Banco de dados NoSQL baseado em documentos. Ele armazena dados em formato JSON-like, proporcionando flexibilidade na modelagem de dados.

# Azure Data Lake
- **Azure Data Lake**: Serviço de armazenamento escalável e seguro no Azure, otimizado para grandes volumes de dados. Ele é projetado para processar dados de qualquer tipo e tamanho para análise e processamento em grande escala.

# Instância Gerenciada de SQL
- **Instância Gerenciada de SQL**: Serviço do Azure que oferece uma instância completa de SQL Server na nuvem. Ele oferece compatibilidade total com o SQL Server e é adequado para migrações de ambientes locais para a nuvem.

# SQL Server em Máquinas Virtuais do Azure que executam o Windows
- **SQL Server em VMs do Azure**: Oferece a execução do SQL Server em máquinas virtuais no Azure, permitindo que os clientes tenham controle total sobre o ambiente do SQL Server, com flexibilidade de configuração e personalização.

# Banco de Dados SQL do Azure
- **Banco de Dados SQL do Azure**: Serviço de banco de dados relacional totalmente gerenciado que oferece alta disponibilidade, escalabilidade automática e backups automatizados. Ele é baseado no mecanismo do Microsoft SQL Server.

# Bancos de Dados OLAP
- **Bancos de Dados OLAP (Online Analytical Processing)**: São projetados para consultas complexas e análises multidimensionais, ideais para cenários de business intelligence (BI). Eles permitem a agregação de grandes volumes de dados e fornecem uma visão consolidada para tomada de decisão.

# Formato ORC
- **Formato ORC (Optimized Row Columnar)**: Formato de arquivo altamente otimizado para armazenamento de dados em colunas, frequentemente utilizado em big data. Ele melhora a eficiência de leitura e escrita, economizando espaço e acelerando as consultas.
