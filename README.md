# Analista_Dados_Oppai

# Explicação e entendimento das implementações feitas:
#### Criação da arquitetura dentro do ambiente Google Cloud.
#### Utilizou-se Cloud Storage como os buckets de ingestão e de ETL.
#### Utilização do Big Query como DW (Data Warehouse) -  No ambiente Big Query usa-se SQL, assim caso seja necessário poderá criar as Views ou fazer joins entre tabelas Fato e Dimensionais.
#### Utilização do Python como linguagem principal, no entanto uma boa alternativa seria o PySpark, Dask ou Polars.
#### Arquivos salvos em parquet e csv.
#### Apliacação do NLP (Processamento de Linguagem Natural) - Rodou-se um algoritimo da qual retorno tipos de sentimentos baseado nos tipos de comentários (Primeiramente foi feito uma transformação para a língua inglesa, devido a biblioteca utilizada).
#### Utilização do Airflow para orquestrar os Dags dos pipelines.
#### Utilização do Postman para caso seja necessário ativar os pipelines por meio de API do AirFlow.
#### Utilização do Redis - A utilização do Redis é uma alternativa viável para a incrementação dos dados futuramente, pois visando o a gravação das 'Datas' na memórias, tornaria o processo mais rápido.
#### Utilização do Power BI para a visualização (Foi feito a conexão do Power BI no Big Query - as conexões pode ser to tipo direct ou import).

## A arquitetura do Datalake proposta:
![Texto Alternativo](Arquitetura_DataLake_GCP.png)
### Camadas LND, Silver e Gold no GCP:
![Texto Alternativo](lnd_silver_gold.png)
### Data Warehouse - BIG QUERY:
![Texto Alternativo](big_query.png)

## Workflow da ingestão e do ETL até DW:
![Texto Alternativo](DAGS_workflows.drawio.png)

