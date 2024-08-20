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
- **Azure Synapse Analytics**: Serviço nativo de análise do Azure criado no Spark  que combina big data e análise de dados empresariais. Ele permite o processamento de consultas SQL e a execução de pipelines de dados em grande escala, fornecendo insights em tempo real. O Stream Analytics permite agregar dados de um período específico antes de serem gravados em um data lake.

# Data Warehouse
- **Data Warehouse**: É um sistema de armazenamento de dados projetado para análise e geração de relatórios. Ele integra dados de várias fontes, estruturados e semiestruturados, otimizado para consultas analíticas e relatórios históricos. Data Warehouses são usados em soluções de BI para suportar decisões empresariais. O **Azure Synapse Analytics** é uma solução de data warehouse, que combina capacidades de processamento de big data e análise de dados empresariais. Os data warehouses usam tabelas de fatos e de dimensões em um esquema em estrela/floco de neve.

# Blobs
- **Blobs**: São objetos de armazenamento no Azure Blob Storage usados para armazenar grandes quantidades de dados não estruturados, como imagens, vídeos, documentos e backups.

# Instruções SQL
- **Instruções SQL**: Conjunto de comandos usados para gerenciar e consultar bancos de dados relacionais.
Algumas instruções:
  - **SELECT - INTO** faz uma inserção
em uma tabela.
  - **SELECT - OVER** determina o particionamento e a ordenação do conjunto de linhas antes que uma função de janela seja aplicada
  - **INSERT - VALUES** insere valores em uma única linha.
  - **SELECT - HAVING** filtra dados.
  - **MERGE**: permite combinar dados de duas tabelas com base em uma condição específica, realizando operações de inserção, atualização ou exclusão em uma única instrução.

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

# HDInsight
- **Azure HDInsight**: serviço do Azure que oferece clusters de big data de código aberto baseados em frameworks populares como Apache Hadoop, Spark, Hive, Kafka, HBase, entre outros. O HDInsight permite processar grandes volumes de dados, realizar análises em tempo real, e executar pipelines de machine learning e ETL em ambientes escaláveis.

# Stream Analytics
O **Stream Analytics** pode lidar com o processamento de fluxo do Kafka para o Data Lake.

# Fontes para processamento de fluxo
Os serviços a seguir são comumente usados para ingerir dados para processamento de fluxo no Azure:

- **Hubs de Eventos do Azure**: um serviço de ingestão de dados que você pode usar para gerenciar filas de dados de eventos, garantindo que cada evento seja processado em ordem, exatamente uma vez.
- **Hub IoT do Azure**: um serviço de ingestão de dados semelhante aos Hubs de Eventos do Azure, mas otimizado para gerenciar dados de eventos de dispositivos da Internet das Coisas (IoT).
- **Azure Data Lake Store Gen 2**: um serviço de armazenamento altamente escalonável que é frequentemente usado em cenários de processamento em lotes, mas que também pode ser usado como fonte de dados de streaming.
- **Apache Kafka**: uma solução de ingestão de dados de código aberto que é comumente usada em conjunto com o Apache Spark. Você pode usar o Azure HDInsight para criar um cluster Kafka.

# Drill Up e Drill Down
- Uma hierarquia permite fazer drill up e fazer drill down em uma dimensão. 
- **Drill Down**: 
  - **Definição**: Processo de aprofundar a análise dos dados, movendo-se de um nível de agregação para níveis mais detalhados.
  - **Exemplo**: Ao visualizar as vendas anuais de uma empresa, o drill down permite que você veja as vendas por trimestre, mês, semana ou até mesmo por dia.
  - **Uso**: Utilizado para explorar causas subjacentes, identificar padrões específicos e obter insights mais detalhados sobre os dados.

- **Drill Up**:
  - **Definição**: Processo oposto ao drill down, movendo-se de um nível de detalhe para um nível mais agregado.
  - **Exemplo**: Se você estiver visualizando as vendas mensais, o drill up pode resumir essas informações para o nível trimestral ou anual.
  - **Uso**: Utilizado para obter uma visão geral dos dados, resumir informações detalhadas e entender tendências em um nível mais amplo.
