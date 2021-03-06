# Data-analytics

[![MIT License](https://img.shields.io/apm/l/atomic-design-ui.svg?)](https://github.com/tterb/atomic-design-ui/blob/master/LICENSEs)
[![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)
[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)
[![author](https://img.shields.io/badge/author-RafaelGallo-red.svg)](https://github.com/RafaelGallo?tab=repositories) 
[![](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-374/) 
[![](https://img.shields.io/badge/R-3.6.0-red.svg)](https://www.r-project.org/)
[![](https://img.shields.io/badge/ggplot2-white.svg)](https://ggplot2.tidyverse.org/)
[![](https://img.shields.io/badge/dplyr-blue.svg)](https://dplyr.tidyverse.org/)
[![](https://img.shields.io/badge/readr-green.svg)](https://readr.tidyverse.org/)
[![](https://img.shields.io/badge/ggvis-black.svg)](https://ggvis.tidyverse.org/)
[![](https://img.shields.io/badge/Shiny-red.svg)](https://shiny.tidyverse.org/)
[![](https://img.shields.io/badge/plotly-green.svg)](https://plotly.com/)
[![](https://img.shields.io/badge/XGBoost-red.svg)](https://xgboost.readthedocs.io/en/stable/#)
[![](https://img.shields.io/badge/Tensorflow-orange.svg)](https://powerbi.microsoft.com/pt-br/)
[![](https://img.shields.io/badge/Keras-red.svg)](https://powerbi.microsoft.com/pt-br/)
[![](https://img.shields.io/badge/CUDA-gree.svg)](https://powerbi.microsoft.com/pt-br/)
[![](https://img.shields.io/badge/Caret-orange.svg)](https://caret.tidyverse.org/)
[![](https://img.shields.io/badge/Pandas-blue.svg)](https://pandas.pydata.org/) 
[![](https://img.shields.io/badge/Matplotlib-blue.svg)](https://matplotlib.org/)
[![](https://img.shields.io/badge/Seaborn-green.svg)](https://seaborn.pydata.org/)
[![](https://img.shields.io/badge/Matplotlib-orange.svg)](https://scikit-learn.org/stable/) 
[![](https://img.shields.io/badge/Scikit_Learn-green.svg)](https://scikit-learn.org/stable/)
[![](https://img.shields.io/badge/Numpy-white.svg)](https://numpy.org/)
[![](https://img.shields.io/badge/PowerBI-red.svg)](https://powerbi.microsoft.com/pt-br/)

![Logo](https://image.freepik.com/vetores-gratis/design-de-fundo-de-malha-de-rede-de-tecnologia-de-visualizacao-de-dados_1017-30516.jpg)


## Projeto

- Projeto voltado para an??lise de dados.


## Stack utilizada

**Programa????o** Python

**Leitura CSV**: Pandas

**An??lise de dados**: Seaborn, Matplotlib



## Vari??veis de Ambiente

Para rodar esse projeto, voc?? vai precisar adicionar as seguintes vari??veis de ambiente no seu .env

Instalando a virtualenv

`pip install virtualenv`

Nova virtualenv

`virtualenv nome_virtualenv`

Ativando a virtualenv

`source nome_virtualenv/bin/activate` (Linux ou macOS)

`nome_virtualenv/Scripts/Activate` (Windows)

Retorno da env

`projeto_py source venv/bin/activate` 

Desativando a virtualenv

`(venv) deactivate` 

Instalando pacotes

`(venv) projeto_py pip install flask`

Instalando as bibliotecas

`pip freeze`


## Instala????o

Instala????o das bibliotecas para esse projeto no python.

```bash
  conda install pandas 
  conda install scikitlearn
  conda install numpy
  conda install scipy
  conda install matplotlib

  python==3.6.4
  numpy==1.13.3
  scipy==1.0.0
  matplotlib==2.1.2
```
Instala????o do Python ?? altamente recomend??vel usar o anaconda para instalar o python. Clique aqui para ir para a p??gina de download do Anaconda https://www.anaconda.com/download. Certifique-se de baixar a vers??o Python 3.6. Se voc?? estiver em uma m??quina Windows: Abra o execut??vel ap??s a conclus??o do download e siga as instru????es. 

Assim que a instala????o for conclu??da, abra o prompt do Anaconda no menu iniciar. Isso abrir?? um terminal com o python ativado. Se voc?? estiver em uma m??quina Linux: Abra um terminal e navegue at?? o diret??rio onde o Anaconda foi baixado. 
Altere a permiss??o para o arquivo baixado para que ele possa ser executado. Portanto, se o nome do arquivo baixado for Anaconda3-5.1.0-Linux-x86_64.sh, use o seguinte comando: chmod a x Anaconda3-5.1.0-Linux-x86_64.sh.

Agora execute o script de instala????o usando.


Depois de instalar o python, crie um novo ambiente python com todos os requisitos usando o seguinte comando

```bash
conda env create -f environment.yml
```
Ap??s a configura????o do novo ambiente, ative-o usando (windows)
```bash
activate "Nome do projeto"
```
ou se voc?? estiver em uma m??quina Linux
```bash
source "Nome do projeto" 
```
Agora que temos nosso ambiente Python todo configurado, podemos come??ar a trabalhar nas atribui????es. Para fazer isso, navegue at?? o diret??rio onde as atribui????es foram instaladas e inicie o notebook jupyter a partir do terminal usando o comando
```bash
jupyter notebook
```
    
## Demo An??lise de dados

```bash
  # Carregando as bibliotecas 
  import pandas as pd
  import seaborn as sns
  import matplotlib.pyplot as plt

  # Carregando o dataset
  data = pd.read_csv("data.csv")
  
  # Visualizando os 5 primeiros itens
  data.head()

  # visualizando linhas e colunas com shape
  data.shape

  # Informa????es das variaveis
  data.info()

  # An??lise de dados
  
  # Gr??fico de barras
  plt.figure(figsize=(20, 10))
  plt.title("Total email real e spam")
  sns.countplot(base["Prediction"])
  plt.xlabel("SPAM REAL")
  plt.ylabel("Total")

  #Gr??fico de pizza
  plt.figure(figsize=(20, 10))

  plt.pie(base.groupby("Prediction")['Prediction'].count(), labels=["SPAM", "REAL"], autopct = "%1.1f%%");
  plt.title("Total de email spam ou real")
  plt.legend(["SPAM", "REAL"])

  #Gr??fico de scatterplot
  plt.figure(figsize=(15.8, 10))
  ax = sns.scatterplot(x="the", y="hou", data = base, hue ="Prediction")
  plt.title("Total email real e spam")
  plt.xlabel("SPAM REAL")
  plt.ylabel("Total")

  # Gr??fico de histrograma
  plt.figure(figsize=(15.8, 10))
  ax = sns.histplot(x="the", y="hou", data = base, hue ="Prediction")
  plt.title("Total email real e spam")
  plt.xlabel("SPAM REAL")
  plt.ylabel("Total")






```


## Melhorias

Que melhorias voc?? fez no seu c??digo? 
- Ex: refatora????es, melhorias de performance, acessibilidade, etc


## Suporte

Para suporte, mande um email para rafaelhenriquegallo@gmail.com

