# Machine Learning Projects

Repositório dedicado aos meus estudos e projetos práticos de Machine Learning, com foco em análise exploratória de dados, preparação de bases, engenharia de atributos, treinamento de modelos e avaliação de desempenho.

A proposta deste repositório é reunir projetos desenvolvidos ao longo da minha jornada de aprendizado em Ciência de Dados, aplicando conceitos de Python, estatística, visualização de dados e algoritmos de Machine Learning em problemas de regressão e classificação com bases públicas.

## Objetivo

Este repositório tem como objetivo documentar minha evolução prática em Machine Learning por meio de projetos organizados, cobrindo etapas como:

- entendimento do problema;
- análise exploratória dos dados;
- tratamento e preparação da base;
- criação e seleção de variáveis;
- treinamento de modelos;
- avaliação de métricas;
- interpretação dos principais resultados e aprendizados.

## Projetos

### Fase 1: Regressão e previsão contínua

#### Projeto 1: Regressão Linear Simples (Baseline)

- **Tema:** Previsão de Custos Médicos
- **Dataset sugerido:** Medical Cost Personal Datasets (Kaggle)
- **Desafio:** prever o custo do seguro médico de uma pessoa com base em idade, IMC e hábitos
- **Conceitos-chave:** correlação, p-valor, interpretação de coeficientes, erro quadrático (RMSE)

#### Projeto 2: Regressão com Regularização (Lasso/Ridge)

- **Tema:** Precificação de Veículos Usados
- **Dataset sugerido:** Used Cars Price Prediction
- **Desafio:** prever o preço de revenda lidando com múltiplas variáveis categóricas, como marca, versão e localização
- **Conceitos-chave:** One-Hot Encoding, multicolinearidade, overfitting vs. underfitting, regularização L1/L2

#### Projeto 3: Regressão Não-Linear (Ensembles)

- **Tema:** Previsão de Preços de Passagens Aéreas
- **Dataset sugerido:** Flight Price Prediction
- **Desafio:** capturar relações complexas e não-lineares, como o efeito de dias até o voo no preço
- **Conceitos-chave:** Random Forest Regressor, XGBoost, comparação de modelos baseados em árvore vs. lineares

### Fase 2: Classificação e decisão

Foco: separar classes, lidar com probabilidade e interpretar decisões dos modelos.

#### Projeto 4: Classificação Multiclasse Simples

- **Tema:** Classificação de Faixa de Preço de Celulares
- **Dataset sugerido:** Mobile Price Classification
- **Desafio:** determinar se um celular é de custo baixo, médio, alto ou muito alto com base nas especificações
- **Conceitos-chave:** Feature Selection, matriz de confusão, acurácia

#### Projeto 5: Support Vector Machines (SVM)

- **Tema:** Reconhecimento de Atividade Humana (HAR)
- **Dataset sugerido:** Human Activity Recognition with Smartphones
- **Desafio:** classificar atividades como andar, sentar e deitar usando dados de sensores
- **Conceitos-chave:** hiperplanos, margens, Kernel Trick (RBF vs Linear), alta dimensionalidade

## Tecnologias utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Statsmodels
- SciPy
- Jupyter Notebook

## Organização dos projetos

Cada projeto segue uma estrutura semelhante, separando dados e notebooks:

- `data/`: bases originais e arquivos derivados do projeto;
- `notebooks/`: análises exploratórias e etapas de modelagem.

Em geral, os notebooks seguem a ordem:

- `01_eda.ipynb`: análise exploratória dos dados;
- `02_*.ipynb`: etapa de modelagem, comparação de algoritmos e avaliação.

## Estrutura do repositório

```text
machine-learning-projects/
├── 01-insurance-medical-cost/
│   ├── data/
│   └── notebooks/
├── 02-car-price-prediction/
│   ├── data/
│   └── notebooks/
├── 03-flight-price-prediction/
│   ├── data/
│   └── notebooks/
├── 04-mobile-price-classification/
│   ├── data/
│   └── notebooks/
├── 05-human-activity-recognition/
│   ├── data/
│   └── notebooks/
└── README.md
```

## Observações

Os projetos foram desenvolvidos principalmente em notebooks, com foco didático e exploratório. Por isso, a ênfase está menos em empacotamento de código e mais no raciocínio analítico, comparação de abordagens e documentação dos aprendizados ao longo de cada estudo.
