# Projeto 3: Flight Price Prediction

## Objetivo do projeto

Este projeto tem como objetivo prever o preço de passagens aéreas a partir de atributos da viagem, como companhia aérea, cidades de origem e destino, horário, número de escalas, antecedência da compra e classe do voo.

Fonte do dataset no Kaggle:

https://www.kaggle.com/datasets/shubhambathwal/flight-price-prediction

## Tema

Previsão de preços de passagens aéreas.

## Desafio

Capturar relações complexas e não lineares entre o preço e variáveis como dias até o voo, companhia aérea, classe e rota.

## Conceitos-chave

- regressão não linear
- ensembles
- Random Forest Regressor
- comparação entre modelos baseados em árvore e modelos lineares

## About Dataset

According to the Kaggle page, the objective of the study is to analyze a flight booking dataset obtained from the Ease My Trip website and apply regression techniques to predict ticket prices.

The original study also proposed statistical analysis to answer practical questions related to airline prices, booking timing and travel characteristics.

## Research Questions

O estudo original destaca perguntas como:

- o preço varia entre companhias aéreas?
- comprar a passagem 1 ou 2 dias antes afeta o preço?
- o horário de partida e chegada influencia o valor?
- origem e destino alteram o preço da passagem?
- existe diferença relevante entre classe econômica e executiva?

## Data collection and methodology

Segundo a descrição do Kaggle:

- os dados foram coletados com a ferramenta `Octoparse`
- a fonte foi o site `Ease My Trip`
- a coleta ocorreu entre `11 de fevereiro` e `31 de março de 2022`
- foram extraídas `300.261` opções distintas de voos

## Dataset

O dataset limpo contém informações de voos entre as 6 principais cidades metropolitanas da Índia e possui `11` variáveis principais.

Na pasta do projeto, os arquivos disponíveis são:

- `Clean_Dataset.csv`
- `business.csv`
- `economy.csv`

## Features

As variáveis descritas na base são:

- `airline`: companhia aérea
- `flight`: código do voo
- `source_city`: cidade de origem
- `departure_time`: faixa de horário de partida
- `stops`: número de escalas
- `arrival_time`: faixa de horário de chegada
- `destination_city`: cidade de destino
- `class`: classe do assento (`Business` ou `Economy`)
- `duration`: duração total do voo em horas
- `days_left`: quantidade de dias entre compra e viagem
- `price`: preço da passagem, variável alvo

## Estrutura do projeto

```text
03-flight-price-prediction/
├── data/
│   ├── Clean_Dataset.csv
│   ├── business.csv
│   └── economy.csv
├── notebooks/
│   ├── 01_eda.ipynb
│   └── 02_regularized_regression.ipynb
└── README.md
```
