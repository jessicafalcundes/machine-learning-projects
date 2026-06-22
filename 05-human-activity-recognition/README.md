# Projeto 5: Human Activity Recognition with Smartphones

## Objetivo do projeto

Este projeto tem como objetivo prever a coluna `Activity` a partir de dados de sensores de smartphone, tratando o problema como uma tarefa de classificação multiclasse.

Fonte do dataset no Kaggle:

https://www.kaggle.com/datasets/uciml/human-activity-recognition-with-smartphones

As atividades previstas são:

- `WALKING`
- `WALKING_UPSTAIRS`
- `WALKING_DOWNSTAIRS`
- `SITTING`
- `STANDING`
- `LAYING`

## About Dataset

The Human Activity Recognition database was built from the recordings of 30 study participants performing activities of daily living (ADL) while carrying a waist-mounted smartphone with embedded inertial sensors. The objective is to classify activities into one of the six activities performed.

## Description of experiment

The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (`WALKING`, `WALKING_UPSTAIRS`, `WALKING_DOWNSTAIRS`, `SITTING`, `STANDING`, `LAYING`) wearing a smartphone (`Samsung Galaxy S II`) on the waist.

Using its embedded accelerometer and gyroscope, the study captured:

- 3-axial linear acceleration
- 3-axial angular velocity

The signals were recorded at a constant rate of `50Hz`.

The experiments were video-recorded to label the data manually. The obtained dataset was randomly partitioned into two sets:

- `70%` of the volunteers for training data
- `30%` of the volunteers for test data

## Signal processing and feature extraction

The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of `2.56 seconds` with `50% overlap` (`128 readings per window`).

The acceleration signal, which contains gravitational and body motion components, was separated using a Butterworth low-pass filter into:

- body acceleration
- gravity acceleration

The gravitational force was assumed to have only low-frequency components, so a filter with cutoff frequency of `0.3 Hz` was used.

From each window, a vector of features was obtained by calculating variables from:

- the time domain
- the frequency domain

## Attribute information

For each record in the dataset, the following is provided:

- Triaxial acceleration from the accelerometer (total acceleration) and the estimated body acceleration
- Triaxial angular velocity from the gyroscope
- A `561`-feature vector with time and frequency domain variables
- Its activity label
- An identifier of the subject who carried out the experiment

## Dicionário de dados resumido

Além das colunas `Activity` e `subject`, o dataset contém centenas de variáveis derivadas dos sinais dos sensores. Os nomes seguem padrões importantes:

- `subject`: identificador do participante
- `Activity`: atividade realizada pelo participante
- prefixo `t`: variável extraída no domínio do tempo
- prefixo `f`: variável extraída no domínio da frequência
- `BodyAcc`: aceleração corporal
- `GravityAcc`: componente de gravidade
- `BodyGyro`: velocidade angular do giroscópio
- `Jerk`: variação brusca do sinal
- `Mag`: magnitude do vetor

Alguns sufixos frequentes:

- `mean()`: média
- `std()`: desvio padrão
- `mad()`: median absolute deviation
- `max()` / `min()`: máximos e mínimos
- `sma()`: signal magnitude area
- `energy()`: energia do sinal
- `iqr()`: intervalo interquartil
- `entropy()`: entropia
- `arCoeff()`: coeficientes autorregressivos
- `correlation()`: correlação entre eixos
- `bandsEnergy()`: energia em bandas de frequência
- `meanFreq()`: frequência média
- `skewness()`: assimetria
- `kurtosis()`: curtose
- `angle(...)`: ângulos entre vetores e componentes de gravidade

## Estrutura do projeto

```text
05-human-activity-recognition/
├── data/
│   ├── train.csv
│   ├── test.csv
│   └── human_activity_predictions.csv
├── notebooks/
│   ├── 01_eda.ipynb
│   └── 02_multiclass_classification.ipynb
└── README.md
```

## Relevant papers

1. Davide Anguita, Alessandro Ghio, Luca Oneto, Xavier Parra and Jorge L. Reyes-Ortiz. *Human Activity Recognition on Smartphones using a Multiclass Hardware-Friendly Support Vector Machine*. International Workshop of Ambient Assisted Living (IWAAL 2012). Vitoria-Gasteiz, Spain. Dec 2012.
2. Davide Anguita, Alessandro Ghio, Luca Oneto, Xavier Parra, Jorge L. Reyes-Ortiz. *Energy Efficient Smartphone-Based Activity Recognition using Fixed-Point Arithmetic*. Journal of Universal Computer Science. Special Issue in Ambient Assisted Living: Home Care. Volume 19, Issue 9. May 2013.
3. Davide Anguita, Alessandro Ghio, Luca Oneto, Xavier Parra and Jorge L. Reyes-Ortiz. *Human Activity Recognition on Smartphones using a Multiclass Hardware-Friendly Support Vector Machine*. 4th International Workshop of Ambient Assited Living, IWAAL 2012, Vitoria-Gasteiz, Spain, December 3-5, 2012. Proceedings. Lecture Notes in Computer Science 2012, pp 216-223.
4. Jorge Luis Reyes-Ortiz, Alessandro Ghio, Xavier Parra-Llanas, Davide Anguita, Joan Cabestany, Andreu Català. *Human Activity and Motion Disorder Recognition: Towards Smarter Interactive Cognitive Environments*. 21st European Symposium on Artificial Neural Networks, Computational Intelligence and Machine Learning, ESANN 2013. Bruges, Belgium, 24-26 April 2013.

## Citation

Davide Anguita, Alessandro Ghio, Luca Oneto, Xavier Parra and Jorge L. Reyes-Ortiz. *A Public Domain Dataset for Human Activity Recognition Using Smartphones*. 21st European Symposium on Artificial Neural Networks, Computational Intelligence and Machine Learning, ESANN 2013. Bruges, Belgium, 24-26 April 2013.
