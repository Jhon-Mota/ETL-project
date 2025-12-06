# ETL de Dados de Carros

Projeto de portfólio em Python que implementa um pipeline ETL (Extract, Transform, Load) para um conjunto de dados de carros, utilizando **Pandas** e **SQLAlchemy** para tratamento dos dados e carga em um banco relacional.

## Objetivo do projeto

- Demonstrar a construção de um pipeline ETL simples e bem estruturado em Python.
- Praticar leitura, limpeza, transformação e carregamento de dados tabulares com Pandas.
- Servir como exemplo de projeto de portfólio para análise/engenharia de dados no GitHub.

## Dataset

- Dataset com informações de carros como: fabricante (`company`), tipo de carroceria (`body-style`), distância entre eixos (`wheel-base`), comprimento (`length`), tipo de motor (`engine-type`), número de cilindros, potência (`horsepower`), consumo médio (`average-mileage`) e preço (`price`).
- Os dados estão organizados em um DataFrame com 61 linhas e 10 colunas, representando diferentes modelos de veículos.

## Pipeline ETL

### 1. Extração (Extract)

- Leitura do dataset em um DataFrame Pandas (por exemplo, a partir de um arquivo CSV ou outra fonte tabular). 
- Organização das colunas relevantes para a análise e para a futura carga em banco.

### 2. Transformação (Transform)

- Ajustes de tipos de dados (numéricos e categóricos) quando necessário.
- Limpeza básica dos dados (remoção de valores ausentes ou inconsistentes, se aplicável).
- Preparação final do DataFrame para envio ao banco de dados (nomes de colunas, formatos, etc.).

### 3. Carga (Load)

- Criação de uma conexão com o banco de dados usando **SQLAlchemy**.
- Escrita do DataFrame em uma tabela SQL por meio do método `DataFrame.to_sql`, permitindo criar ou substituir a tabela de destino.

## Tecnologias utilizadas

- **Linguagem:** Python  
- **Bibliotecas principais:**  
  - `pandas` para manipulação e transformação dos dados.
  - `sqlalchemy` para conexão e escrita dos dados no banco relacional.
- **Banco de dados:** qualquer banco compatível com SQLAlchemy (foi utilizado SQL Server para este projeto).

