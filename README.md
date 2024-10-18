# Tipos de dados
- **Dados Estruturados:** Dados organizados em um formato pré-definido, como tabelas de bancos de dados com colunas e tipos de dados específicos.
- **Dados Semiestruturados:** Dados parcialmente estruturados, como JSON ou XML, que possuem uma organização hierárquica, mas não seguem um esquema rígido.
- **Dados Não Estruturados:** Dados que não possuem uma organização ou estrutura definida, como vídeos, imagens, ou textos livres.

# Tipos de banco de dados
- **Bancos de Dados Relacionais:** Estruturados em tabelas com chaves primárias e estrangeiras, usando SQL para consultas. Ex.: MySQL, PostgreSQL.
- **Bancos de Dados NoSQL:** Flexíveis em estrutura, usados para dados distribuídos e de grande escala. Ex.: MongoDB, Cassandra, Cosmos DB.
- **Diferença entre Bancos de Dados NoSQL e Relacionais**: Bancos NoSQL não utilizam esquema fixo e são mais flexíveis, enquanto os relacionais seguem um esquema rígido com tabelas, colunas e tipos de dados definidos.
- **Casos de Uso de Dados Não Relacionais**: Ideal para grandes volumes de dados não estruturados ou semiestruturados, como redes sociais, catálogos de produtos e dados de IoT.

# Tipos de análise de dados
- **Descritiva:** O que acontece?
- **Diagnóstica:** Por que acontecem?
- **Preditiva:** O que vai acontecer?
- **Prescritiva:** Que ações devemos tomar?
- [Ver mais](https://www.microsoft.com/pt-br/microsoft-365/excel/data-analysis)

# Níveis de complexidade na estruturação de dados JSON
## Exemplo de uma matriz aninhada (nested array):
``` json
{
  "nome": "Felipe",
  "notas": [
    [8, 9, 7],
    [6, 8, 10],
    [9, 7, 8]
  ]
}
```
Neste exemplo, a chave `notas` possui uma matriz que contém outras matrizes dentro.

## Exemplo de um objeto aninhado (nested object):
``` json
{
  "nome": "Felipe",
  "endereco": {
    "rua": "Av. Principal",
    "numero": 123,
    "cidade": {
      "nome": "São Paulo",
      "estado": "SP"
    }
  }
}
```
Neste caso, o objeto `endereco` contém outro objeto dentro dele (o objeto `cidade`).

## Exemplo de um objeto raiz (root object):
``` json
{
  "id": 1,
  "titulo": "Introdução ao JSON",
  "autor": "Felipe Santos"
}
```
Aqui, o objeto representado no nível mais alto é o objeto raiz, que contém pares chave-valor diretamente sem aninhamento.

# Diferença entre Schema Estrela e Floco de neve (star e snowflake)

| Característica          | Esquema Estrela            | Esquema Floco de Neve      |
|-------------------------|----------------------------|----------------------------|
| Estrutura               | Dimensões desnormalizadas   | Dimensões normalizadas      |
| Complexidade            | Simples, menos tabelas      | Complexo, mais tabelas      |
| Desempenho de consulta  | Geralmente mais rápido      | Geralmente mais lento       |
| Redundância de dados    | Mais redundante             | Menos redundante            |

# Tipos de instrução SQL
  - **DQL>** Linguagem de consulta de dados
  - **DML:** Linguagem de manipulação de dados
  - **DDL:** Linguagem de definição de dados
  - **DCL:** Linguagem de controle de dados
  - **DTL:** Linguagem de transição de dados
<img src="https://arquivo.devmedia.com.br/artigos/destaques/guia/SQL.png" alt="Texto Alternativo" width="500"/>

## Outras
  - **SELECT - INTO** faz uma inserção em uma tabela.
  - **SELECT - OVER** determina o particionamento e a ordenação do conjunto de linhas antes que uma função de janela seja aplicada
  - **INSERT - VALUES** insere valores em uma única linha.
  - **SELECT - HAVING** filtra dados.
  - **MERGE**: permite combinar dados de duas tabelas com base em uma condição específica, realizando operações de inserção, atualização ou exclusão em uma única instrução.
[Ver mais](https://learn.microsoft.com/pt-br/sql/t-sql/queries/select-into-clause-transact-sql?view=sql-server-ver16)

# Conceitos de Análise de Dados
- **Processamento de Dados para Análise**:
  - **ETL** (Extract, Transform, Load): Processo de extração, transformação e carregamento de dados em um sistema de destino.
  - **ELT** (Extract, Load, Transform): Processo em que os dados são carregados no sistema de destino antes de serem transformados.
- **Armazenamento de Dados no Azure**:
  - Azure Data Lake
  - Armazenamento Blob
- **Ferramentas de Análise de Dados no Azure**:
  - Azure Synapse Analytics
  - Power BI
  - Databricks

# Azure Data Lake
Serviço de armazenamento escalável e seguro no Azure, otimizado para grandes volumes de dados. Ele é projetado para processar dados de qualquer tipo e tamanho para análise e processamento em grande escala. O Data Lake Storage Gen2 é usado para armazenar grandes quantidades de dados a serem processados por serviços como o Databricks, o Azure Synapse Analytics e o HDInsight. [Ver mais](https://learn.microsoft.com/pt-br/training/modules/explore-provision-deploy-non-relational-data-services-azure/3-azure-data-lake-gen2)

# Delta Lake
O Delta Lake é uma camada de armazenamento de código aberto que adiciona suporte ao Data Lake Storage para consistência transacional.
É um serviço de análise e banco de dados de alto desempenho otimizado para ingestão e consulta de dados em lote ou streaming com um elemento de série temporal e que pode ser usado como um serviço autônomo do Azure ou como um tempo de execução do Azure Synapse Data Explorer em um espaço de trabalho do Azure Synapse Analytics.

# OLTP (Online Transaction Processing)
OLTP refere-se ao Processamento de Transações Online.
O trabalho executado por sistemas transacionais é geralmente conhecido como OLTP (Processamento de Transações Online).
Os sistemas OLTP normalmente são usados para dar suporte a aplicativos dinâmicos que processam dados de negócios, geralmente chamados de aplicativos de LOB (linha de negócios).
As soluções OLTP dependem de um sistema de banco de dados no qual o armazenamento de dados é otimizado para operações de leitura e gravação para dar suporte a cargas de trabalho transacionais nas quais os registros de dados são criados, recuperados, atualizados e excluídos (essas operações são geralmente chamadas de CRUD).

# OLAP (Online Analytical Processing)
Bancos de Dados OLAP (Processamento Analítico Online) São projetados para consultas complexas e análises multidimensionais, ideais para cenários de business intelligence (BI). Eles permitem a agregação de grandes volumes de dados e fornecem uma visão consolidada para tomada de decisão.
OLAP é usado para análise de dados, suporte à decisão e criação de relatórios. Diferente do OLTP, o OLAP é otimizado para consultas complexas e análise de dados históricos.

# Armazenamento de chave/valor
Um armazenamento de chave/valor é usado para pesquisas simples baseadas em uma chave única para obter um valor único.  permite armazenar dados em um formato de duas colunas sem exigir um sistema de gerenciamento de dados complexo. O armazenamento de tabelas é usado para armazenar pares de chave/valor em partições. [Ver mais](https://learn.microsoft.com/pt-br/training/modules/explore-provision-deploy-non-relational-data-services-azure/5-azure-tables)

# Índice
A criação de um índice permite que você pesquise dados em uma tabela com mais eficiência. Em uma tabela que contém poucas linhas, o uso do índice provavelmente não será mais eficiente do que simplesmente ler a tabela inteira e localizar as linhas solicitadas pela consulta (nesse caso, o otimizador de consulta ignorará o índice). No entanto, quando uma tabela tem muitas linhas, os índices podem melhorar drasticamente o desempenho das consultas.

# Azure Synapse Analytics
Serviço nativo de análise do Azure criado no Spark  que combina big data e análise de dados empresariais. Ele permite o processamento de consultas SQL e a execução de pipelines de dados em grande escala, fornecendo insights em tempo real. O Stream Analytics permite agregar dados de um período específico antes de serem gravados em um data lake.

# Data Warehouse
Sistema de armazenamento de dados projetado para análise e geração de relatórios. Ele integra dados de várias fontes, estruturados e semiestruturados, otimizado para consultas analíticas e relatórios históricos. Data Warehouses são usados em soluções de BI para suportar decisões empresariais. O **Azure Synapse Analytics** é uma solução de data warehouse, que combina capacidades de processamento de big data e análise de dados empresariais. Os data warehouses usam tabelas de fatos e de dimensões em um esquema em estrela/floco de neve.

# Blobs
Objetos de armazenamento no Azure Blob Storage usados para armazenar grandes quantidades de dados não estruturados, como imagens, vídeos, documentos e backups. Os **blobs de páginas** são otimizados para acesso aleatório e usados para VHDs [Ver mais](https://learn.microsoft.com/pt-br/training/modules/explore-provision-deploy-non-relational-data-services-azure/2-azure-blob-storage)

# Apache Gremlin
Linguagem de consulta usada para trabalhar com bancos de dados de grafos. Ele permite consultas complexas em estruturas de dados de grafos, que são compostas de vértices e arestas.
O Gremlin é usado para dados em um grafo. As entidades são definidas como vértices que formam nós. Os nós são conectados por bordas que representam relações.

# Apache Cassandra
Banco de dados NoSQL altamente escalável e distribuído, projetado para lidar com grandes volumes de dados em múltiplos servidores, sem pontos de falha. A API do Cassandra é consultada usando SQL. 

# Apache Hadoop
É uma plataforma de código aberto usada para processar e armazenar grandes quantidades de dados. Ele funciona distribuindo esses dados por vários computadores e analisando-os de forma paralela. Essa estrutura permite lidar com grandes volumes de dados de maneira eficiente, mesmo em ambientes com hardware comum.

# CosmosDB
Banco de dados NoSQL distribuído globalmente que oferece suporte a vários modelos de dados (chave-valor, documento, gráfico, etc.). Ele é conhecido por sua baixa latência e alta disponibilidade.

# MongoDB
Banco de dados NoSQL baseado em documentos. Ele armazena dados em formato JSON-like, proporcionando flexibilidade na modelagem de dados. A API do MongoDB também armazena dados no formato BSON.

# PostgreSQL
O PostgreSQL é um banco de dados de objetos híbrido e relacional. Você pode armazenar dados em tabelas relacionais ou armazenar tipos de dados personalizados com propriedades não relacionais.

# Azure Data Explorer
O Data Explorer é usado para a análise de grandes quantidades de dados de log de texto, sites e dispositivos IoT e usa uma linguagem de consulta comum. É um serviço de análise e banco de dados de alto desempenho otimizado para ingestão e consulta de dados em lote ou streaming com um elemento de série temporal e que pode ser usado como um serviço autônomo do Azure ou como um tempo de execução do Azure Synapse Data Explorer em um espaço de trabalho do Azure Synapse Analytics.

# Data Factory
O Data Factory permite orquestrar o fluxo de dados sem codificação usando pipelines.

# Instância Gerenciada de SQL
É um serviço de plataforma como serviço (PaaS) que oferece uma instância completa de SQL Server na nuvem. Ele oferece compatibilidade total com o SQL Server 2016 e é adequado para migrações de ambientes locais para a nuvem. Permite que você migre um servidor do SQL inteiro para a nuvem sem a necessidade de gerenciar a infraestrutura depois da migração. 

# SQL Server em Máquinas Virtuais do Azure que executam o Windows
Oferece a execução do SQL Server em máquinas virtuais no Azure, permitindo que os clientes tenham controle total sobre o ambiente do SQL Server, com flexibilidade de configuração e personalização.

# SQL no Edge
É otimizado para cenários de IoT que devem funcionar com o fluxo de dados de série temporal.

# Banco de Dados SQL do Azure
Serviço de banco de dados relacional totalmente gerenciado que oferece alta disponibilidade, escalabilidade automática e backups automatizados. Ele é baseado no mecanismo do Microsoft SQL Server. O Banco de Dados SQL do Azure é uma instância de SQL de PaaS sem servidor. Permite provisionar um banco de dados individual em um servidor dedicado e tem escalabilidade sob demanda.

É um serviço gerenciado e sem servidor, que evita o uso de licenças do Windows Server e permite que cada carga de trabalho tenha sua própria instância do serviço usado.

Permite criar um banco de dados individual que pode escalar verticalmente e reduzir verticalmente sem tempo de inatividade.

# Formato ORC
Optimized Row Columnar, formato de arquivo altamente otimizado para armazenamento de dados em colunas, frequentemente utilizado em big data. Ele melhora a eficiência de leitura e escrita, economizando espaço e acelerando as consultas.

# HDInsight
Serviço do Azure que oferece clusters de big data de código aberto baseados em frameworks populares como Apache Hadoop, Spark, Hive, Kafka, HBase, entre outros. O HDInsight permite processar grandes volumes de dados, realizar análises em tempo real, e executar pipelines de machine learning e ETL em ambientes escaláveis. O HDInsight é usado para processar grandes quantidades de dados usando o Hadoop. 

# Stream Analytics
O **Stream Analytics** pode lidar com o processamento de fluxo do Kafka para o Data Lake. Permite agregar dados em uma janela de tempo específica antes que os dados sejam gravados em um data lake.

# Fontes para processamento de fluxo
Os serviços a seguir são comumente usados para ingerir dados para processamento de fluxo no Azure:
- **Hubs de Eventos do Azure**: um serviço de ingestão de dados que você pode usar para gerenciar filas de dados de eventos, garantindo que cada evento seja processado em ordem, exatamente uma vez.
- **Hub IoT do Azure**: um serviço de ingestão de dados semelhante aos Hubs de Eventos do Azure, mas otimizado para gerenciar dados de eventos de dispositivos da Internet das Coisas (IoT).
- **Azure Data Lake Store Gen 2**: um serviço de armazenamento altamente escalonável que é frequentemente usado em cenários de processamento em lotes, mas que também pode ser usado como fonte de dados de streaming.
- **Apache Kafka**: uma solução de ingestão de dados de código aberto que é comumente usada em conjunto com o Apache Spark. Você pode usar o Azure HDInsight para criar um cluster Kafka.

# Dimensões
As dimensões são usadas para agregar dados. Entidades que serão usadas para fazer a agregação.

# O que é Drill Up e Drill Down?
- Uma hierarquia permite fazer drill up e fazer drill down em uma dimensão. 
- **Drill Down**: 
  - **Definição**: Processo de aprofundar a análise dos dados, movendo-se de um nível de agregação para níveis mais detalhados.
  - **Exemplo**: Ao visualizar as vendas anuais de uma empresa, o drill down permite que você veja as vendas por trimestre, mês, semana ou até mesmo por dia.
  - **Uso**: Utilizado para explorar causas subjacentes, identificar padrões específicos e obter insights mais detalhados sobre os dados.

- **Drill Up**:
  - **Definição**: Processo oposto ao drill down, movendo-se de um nível de detalhe para um nível mais agregado.
  - **Exemplo**: Se você estiver visualizando as vendas mensais, o drill up pode resumir essas informações para o nível trimestral ou anual.
  - **Uso**: Utilizado para obter uma visão geral dos dados, resumir informações detalhadas e entender tendências em um nível mais amplo.

# Lift and Shift
Estratégia de migração na qual aplicativos e workloads são transferidos de um ambiente on-premises (ou de outro provedor de nuvem) para a nuvem da Microsoft Azure sem grandes modificações ou refatoração. O objetivo é mover a aplicação da maneira mais rápida e simples possível, mantendo sua arquitetura original.
 
# O que é um pipeline?
Sequência automatizada de etapas ou processos que são executados em ordem para alcançar um objetivo específico, como a construção, teste, e entrega de software. É uma maneira de automatizar tarefas repetitivas e garantir que cada etapa seja executada de forma consistente e eficiente. [Ver mais](https://learn.microsoft.com/pt-br/training/modules/examine-components-of-modern-data-warehouse/3-data-ingestion-pipelines)

# O que é Normalização e Desnormalização?
- **Normalização**: É um processo para reduzir a duplicação de dados. Isso pode ser feito separando entidades em suas próprias tabelas e estabelecendo relações entre as tabelas.[Ver mais](https://learn.microsoft.com/pt-br/training/modules/explore-relational-data-offerings/3-normalization)
- **Desnormalização**: Combinação de dados normalizados para melhorar o desempenho de leitura, mesmo que isso aumente a redundância.

# O que é um Procedimento armazenado?
Um procedimento armazenado pode encapsular qualquer tipo de lógica de negócios que possa ser reutilizado no aplicativo. Um procedimento armazenado pode modificar dados existentes, bem como adicionar novas entradas a tabelas. Um procedimento armazenado pode ser executado em um aplicativo, bem como no servidor. [Ver mais](https://learn.microsoft.com/pt-br/training/modules/explore-relational-data-offerings/5-database-objects)

# O que é o processamento em lote?
Usado para executar análises complexas. O processamento em lote manipula uma grande quantidade de dados de cada vez. O processamento em lote geralmente é medido em minutos e horas.

# O que é uma Instância Gerenciada?
Uma instância hospedada do SQL Server com manutenção automatizada, que permite uma configuração mais flexível do que o BD de SQL do Azure, mas com mais responsabilidade administrativa para o proprietário.

# O que é um pool?
Em ambientes como Apache Spark e SQL, o conceito de *pool* também se aplica de maneira específica para gerenciar e otimizar o uso de recursos computacionais.
Pool elástico: recurso que permite a gestão de múltiplos bancos de dados individuais de forma conjunta.

## **Apache Spark: Pool de Recursos (Resource Pools)**
No Apache Spark, um *pool* de recursos é utilizado para gerenciar como os recursos (CPU, memória) são distribuídos entre diferentes tarefas ou jobs. Isso é particularmente útil em ambientes com múltiplos usuários ou aplicativos que compartilham o mesmo cluster.

- **Exemplo de uso**: Se você tiver dois aplicativos rodando simultaneamente em um cluster Spark, pode criar dois *pools* de recursos para garantir que ambos recebam uma parte justa dos recursos do cluster. Um *pool* pode ser configurado para alocar, por exemplo, 60% dos recursos para uma tarefa mais importante e 40% para uma menos crítica.

## **SQL: Pool de Conexões (Connection Pool)**
Em SQL, especialmente em sistemas de bancos de dados, um *pool de conexões* é um conjunto de conexões ao banco de dados que são mantidas ativas para reutilização. Isso melhora o desempenho das aplicações, pois evita o custo associado a criar e destruir conexões para cada interação com o banco de dados.

- **Exemplo de uso**: Suponha que você tenha uma aplicação web que realiza várias consultas ao banco de dados. Em vez de abrir e fechar uma nova conexão a cada consulta, a aplicação utiliza o *pool de conexões* para pegar uma conexão já existente, executar a consulta e depois devolver a conexão ao *pool* para ser reutilizada.

Em ambos os casos, o objetivo do *pool* é otimizar o uso de recursos, evitando desperdício e melhorando o desempenho geral do sistema.

# Administradores de Banco de Dados
Gerenciam bancos de dados, atribuindo permissões aos usuários, armazenando cópias de backup de dados e restaurando dados em caso de falhas.

# Engenheiros de dados
Grenciam a infraestrutura e os processos de integração de dados em toda a organização, aplicando rotinas de limpeza de dados, identificando regras de governança de dados e implementando pipelines para transferir e transformar dados entre sistemas.

# Analistas de Dados
Exploram e analisam dados para criar visualizações e gráficos que permitem que as organizações tomem decisões informadas.
