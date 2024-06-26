# FeatureEngineeringML
Este repositório contém um projeto de engenharia de características e análise de dados usando PySpark e SQL. O objetivo é criar variáveis explicativas a partir de dados de transações e informações cadastrais de clientes para melhorar os modelos de machine learning, com foco em prever o churn (taxa de evasão de clientes). O projeto inclui análises iniciais, criação de variáveis históricas e categóricas, e combinações de dados para fornecer insights valiosos sobre o comportamento dos clientes.

## 1. Principais Tecnologias:

* PySpark
* SQL

## 2. Objetivos:

* Analisar dados de transações e churn.
* Criar variáveis explicativas para modelos de machine learning.

## 3. Descrição das tabelas: 

### 3.1 df_transacoes

A tabela df_transacoes é detalhada em nível de transação, fornecendo uma visão detalhada dos comportamentos de compra e uso do serviço. E vai se relacionar com a tabela 'df_publico' através do 'ID_Cliente'

![image](https://github.com/danielreinaux/FeatureEngineeringML/assets/91274263/937bd260-4343-4889-a6b2-d2edaf868b44)



E

### 3.2 df_publico

Contém informações demográficas, e de uso de serviço dos clientes.
Essa tabela é essencial para entender o perfil dos clientes, e identificar padrões relacionados ao cancelamento do serviço (churn)

![image](https://github.com/danielreinaux/FeatureEngineeringML/assets/91274263/d4d3c946-3d47-468d-b783-05832309ef62)



## 4. Análises Iniciais

As análises iniciais são cruciais para entender o contexto e a qualidade dos dados, identificando padrões preliminares.

### 4.1 Contagem de Transações por Cliente

A contagem de transações por cliente vai nos permitir identificar quantas transações cada cliente realizou:

![image](https://github.com/danielreinaux/FeatureEngineeringML/assets/91274263/f4906dcb-0e9d-43b4-b4e7-72cdf314e3fb)

### 4.2 Valor Médio das Transações por Cliente

Vai calcular o valor médio das transações por cliente, ajudando a entender o ticket médio de cada cliente.
Essa métrica é fundamental para entender quais clientes são mais valiosos para o negócio, e pode ajudar a direcionar estratégias de marketing e retenção:

![image](https://github.com/danielreinaux/FeatureEngineeringML/assets/91274263/846735c1-2254-4296-ba3c-bf371ba54fe8)

## 5. Criando Variáveis Explicativas

### 5.1 Frequência de Compra Mensal:

A frequência de compra mensal ajuda a entender com que regularidade o cliente faz transações. Clientes que compram com maior frequência tendem a se rmais engajados e menos propensos ao Churn

![image](https://github.com/danielreinaux/FeatureEngineeringML/assets/91274263/3fe96dde-0823-4a84-af2f-22da64b5ceeb)

### 5.2 Total Gasto:

Essa variável ajudar a entender quais os clientes que mais gastam. Clientes que gastam mais são geralmente mais valiosos e suas ações são essenciais para o sucesso do negócio

![image](https://github.com/danielreinaux/FeatureEngineeringML/assets/91274263/c4378578-f38c-46b2-9722-c4486a5a6430)

### 

