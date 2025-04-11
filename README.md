# 🌍 Análise de Indicadores de Mudanças Climáticas com PySpark no Databricks

Este repositório contém o notebook desenvolvido na plataforma **Databricks Community**, utilizando a linguagem **PySpark** para construção de um pipeline de dados com base na arquitetura **Medalhão** (Bronze, Prata e Ouro). O objetivo do projeto é realizar a coleta, modelagem, carga e análise de dados sobre variação de temperatura da superfície terrestre a partir de um conjunto disponibilizado pela **FAO (Food and Agriculture Organization of the United Nations)**.

O pipeline contempla as seguintes etapas:

- Importação e armazenamento de dados no **DBFS (Databricks File System)**;
- Criação de tabelas nas camadas Bronze (dados brutos), Prata (dados tratados) e Ouro (dados prontos para análise);
- Transformações com PySpark, incluindo unpivot, limpeza e enriquecimento dos dados;
- Modelagem do banco de dados em **esquema estrela**, seguindo boas práticas de Data Warehousing;
- Execução de consultas SQL para responder a perguntas analíticas sobre o comportamento das anomalias de temperatura;
- Elaboração de um **catálogo de dados** com informações detalhadas sobre cada atributo, regras de validação, entidades e relacionamentos;
- Geração de visualizações e diagramas ER para auxiliar na compreensão da modelagem.

> ⚠️ Para manter o notebook leve e de fácil leitura, todas as exibições de tabelas foram limitadas a **5 linhas**.

## 📁 Arquivos no repositório

- `climate_change_analysis.ipynb` – Notebook principal com o pipeline completo em PySpark e SQL. Nele estão incluídas as explicações detalhadas sobre a modelagem do banco de dados e todas as análises realizadas via SQL.
- `catalogo_dados_temperature_change_on_land.xlsx` – Catálogo de dados completo, contendo descrição dos atributos, domínios, validações, entidades, relacionamentos e chaves.
- Imagens auxiliares (.png) – Diagramas ER e artefatos gerados durante a documentação.

## 📊 Fonte dos Dados

Os dados utilizados são provenientes do conjunto **"Temperature change on land"** disponível no site da FAOSTAT, cobrindo o período de **1961 a 2022**. As informações representam anomalias de temperatura da superfície terrestre em relação à média histórica do período **1951–1980**, com base na série **GISTEMP** distribuída pela **NASA-GISS** (Goddard Institute for Space Studies).

---


