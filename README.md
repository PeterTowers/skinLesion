# Projeto de pesquisa
## Universidade de Brasília

CIC0193 - Fundamentos de Sistemas Inteligentes

Professor: Vinicius Borges

Aluno: Pedro Lucas Silva Haga Torres

Matrícula: 16/0141575

Brasília, 04 de novembro de 2021.

## Classificação multiclasse de imagens dermatoscópicas de lesão de pele

[Base de dados (ISIC Challenge 2019)](https://challenge2019.isic-archive.com/)

## Conteúdos relevantes do repositório

### Artigo
Está salvo como [artigo_PedroTorres_160141575.pdf](https://github.com/PeterTowers/skinLesion/blob/fund_sist_inteligentes/artigo_PedroTorres_160141575.pdf)

### Notebooks
Códigos relativos ao préprocessamento dos dados foi realizado no notebook [skinLesion_preprocessing.ipynb](https://github.com/PeterTowers/skinLesion/blob/fund_sist_inteligentes/skinLesion_preprocessing.ipynb).

Foram treinados dois modelos de classificação utilizando redes EfficientNet-B2 para averiguar o melhor otimizador (Adam ou SGD com Nesterov) para o problema:

#### Adam
O modelo utilizando Adam foi treinado integralmente no **Google Colab**, e o notebook contendo o código utilizado está no arquivo [effNet-B2_adam_trainingPipeline.ipynb](https://github.com/PeterTowers/skinLesion/blob/fund_sist_inteligentes/effNet-B2_adam_trainingPipeline.ipynb). Os modelos salvos e o histórico de treinamento desse modelos estão no diretório `models/adam/`. A versão do TensorFlow para esse modelo é a 2.6.0.

#### SGD + Nesterov
O modelo utilizando SGD foi treinado integralmente **localmente**, e o notebook contendo o código utilizado está no arquivo [effNet-B2_nesterov_localTrainingPipeline.ipynb](https://github.com/PeterTowers/skinLesion/blob/fund_sist_inteligentes/effNet-B2_nesterov_localTrainingPipeline.ipynb). Os modelos salvos e o histórico de treinamento desse modelos estão no diretório `models/nesterov/`. A versão do TensorFlow para esse modelo é a 2.4.1. Gostaria de ter utilizado a 2.6.0 em ambos, porém, tive dificuldades em atualizar a versão em minha máquina. O modelo foi treinado localmente pois também tive dificuldades com o Google Colab.
