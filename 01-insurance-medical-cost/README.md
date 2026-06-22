# Projeto 1: Insurance Medical Cost

## Objetivo do projeto

Este projeto tem como objetivo prever o custo individual do seguro médico a partir de informações pessoais e hábitos de vida, tratando o problema como uma tarefa de regressão.

Fonte do dataset no Kaggle:

https://www.kaggle.com/datasets/mirichoi0218/insurance

## Tema

Previsão de custos médicos.

## Desafio

Estimar o valor de `charges` com base em variáveis como idade, IMC, tabagismo, número de dependentes e região de residência.

## Conceitos-chave

- regressão linear simples e baseline
- correlação
- p-valor
- interpretação de coeficientes
- RMSE

## About Dataset

This dataset is based on the public-domain datasets referenced in the book *Machine Learning with R*, by Brett Lantz. According to the Kaggle page, the original files needed cleaning and recoding to match the format used in the book.

The central question behind the dataset is:

**Can you accurately predict insurance costs?**

## Context

The dataset contains personal and demographic information about insurance beneficiaries in the United States, along with the medical costs charged by the health insurance.

## Content

The main columns are:

- `age`: age of primary beneficiary
- `sex`: insurance contractor gender (`female`, `male`)
- `bmi`: Body Mass Index, an objective index of body weight relative to height
- `children`: number of children or dependents covered by health insurance
- `smoker`: smoking status
- `region`: beneficiary residential area in the US (`northeast`, `southeast`, `southwest`, `northwest`)
- `charges`: individual medical costs billed by health insurance

## Dicionário de dados resumido

- `age`: idade do beneficiário principal
- `sex`: sexo do beneficiário
- `bmi`: índice de massa corporal
- `children`: quantidade de dependentes cobertos
- `smoker`: indica se a pessoa é fumante
- `region`: região de residência nos Estados Unidos
- `charges`: custo individual cobrado pelo seguro de saúde

## Estrutura do projeto

```text
01-insurance-medical-cost/
├── data/
│   └── insurance.csv
├── notebooks/
│   ├── 01_eda.ipynb
│   └── 02_linear_regression.ipynb
└── README.md
```
