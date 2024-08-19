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
