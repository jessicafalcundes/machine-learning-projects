# Projeto 4: Mobile Price Classification

## Objetivo do projeto

Este projeto tem como objetivo prever a faixa de preço de celulares a partir de suas especificações técnicas, tratando o problema como uma tarefa de classificação multiclasse.

Fonte do dataset no Kaggle:

https://www.kaggle.com/datasets/iabhishekofficial/mobile-price-classification

## Tema

Classificação de faixa de preço de celulares.

## Desafio

Determinar se um celular pertence a uma faixa de preço baixa, média, alta ou muito alta com base em atributos como bateria, memória, resolução de tela, câmeras e conectividade.

## Conceitos-chave

- classificação multiclasse
- feature selection
- matriz de confusão
- acurácia
- comparação entre modelos clássicos

## About Dataset

According to the Kaggle page, the dataset is built around the following business problem:

Bob has started his own mobile company and wants to compete with large brands such as Apple and Samsung. He collected data about mobile phones and needs help estimating the price range of new devices based on their technical specifications.

The goal is not to predict the exact selling price, but rather a **price range**.

## Context

O dataset relaciona características técnicas de celulares com a variável alvo `price_range`, que representa a faixa de preço do aparelho.

## Base utilizada no projeto

Os arquivos disponíveis nesta pasta são:

- `train.csv`
- `test.csv`
- `mobile_price_predictions.csv`

As variáveis observadas na base de treino incluem atributos como:

- `battery_power`
- `blue`
- `clock_speed`
- `dual_sim`
- `fc`
- `four_g`
- `int_memory`
- `m_dep`
- `mobile_wt`
- `n_cores`
- `pc`
- `px_height`
- `px_width`
- `ram`
- `sc_h`
- `sc_w`
- `talk_time`
- `three_g`
- `touch_screen`
- `wifi`
- `price_range`

## Dicionário de dados resumido

- `battery_power`: capacidade da bateria
- `blue`: indica presença de bluetooth
- `clock_speed`: velocidade do processador
- `dual_sim`: indica se o aparelho aceita dois chips
- `fc`: resolução da câmera frontal
- `four_g`: suporte a 4G
- `int_memory`: memória interna
- `m_dep`: profundidade do aparelho
- `mobile_wt`: peso
- `n_cores`: número de núcleos do processador
- `pc`: resolução da câmera principal
- `px_height` / `px_width`: resolução da tela em pixels
- `ram`: memória RAM
- `sc_h` / `sc_w`: dimensões da tela
- `talk_time`: tempo de conversa
- `three_g`: suporte a 3G
- `touch_screen`: indica tela sensível ao toque
- `wifi`: suporte a Wi-Fi
- `price_range`: faixa de preço, variável alvo

## Estrutura do projeto

```text
04-mobile-price-classification/
├── data/
│   ├── train.csv
│   ├── test.csv
│   └── mobile_price_predictions.csv
├── notebooks/
│   ├── 01_eda.ipynb
│   └── 02_multiclass_classification.ipynb
└── README.md
```
