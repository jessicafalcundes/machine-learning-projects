# Projeto 2: Used Cars Price Prediction

## Objetivo do projeto

Este projeto tem como objetivo prever o preço de revenda de veículos usados a partir de atributos técnicos e comerciais, tratando o problema como uma tarefa de regressão.

Fonte do dataset no Kaggle:

https://www.kaggle.com/datasets/avikasliwal/used-cars-price-prediction

## Tema

Precificação de veículos usados.

## Desafio

Prever o preço de revenda lidando com múltiplas variáveis categóricas e numéricas, como modelo, localização, tipo de combustível, transmissão e quilometragem.

## Conceitos-chave

- regressão com regularização
- One-Hot Encoding
- multicolinearidade
- overfitting vs. underfitting
- regularização L1/L2

## About Dataset

Na página do Kaggle, este dataset aparece com a observação:

**No description available**

Por isso, a interpretação abaixo foi organizada com base na estrutura local da base utilizada no projeto.

## Base utilizada no projeto

Os arquivos disponíveis nesta pasta são:

- `train-data.csv`
- `test-data.csv`

As colunas observadas na base são:

- `Name`
- `Location`
- `Year`
- `Kilometers_Driven`
- `Fuel_Type`
- `Transmission`
- `Owner_Type`
- `Mileage`
- `Engine`
- `Power`
- `Seats`
- `New_Price`
- `Price`

Há também uma coluna inicial sem nome, que funciona como identificador/índice vindo do arquivo original.

## Dicionário de dados resumido

- `Name`: nome ou versão do veículo
- `Location`: cidade/localização do anúncio
- `Year`: ano do veículo
- `Kilometers_Driven`: quilometragem rodada
- `Fuel_Type`: tipo de combustível
- `Transmission`: tipo de transmissão
- `Owner_Type`: tipo ou histórico de proprietário
- `Mileage`: consumo/rendimento do veículo
- `Engine`: capacidade do motor
- `Power`: potência declarada
- `Seats`: número de assentos
- `New_Price`: preço do veículo novo, quando disponível
- `Price`: preço de revenda, variável alvo

## Estrutura do projeto

```text
02-car-price-prediction/
├── data/
│   ├── train-data.csv
│   └── test-data.csv
├── notebooks/
│   ├── 01_eda.ipynb
│   └── 02_regularized_regression.ipynb
└── README.md
```
