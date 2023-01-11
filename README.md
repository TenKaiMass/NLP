# Projet NLP detection commentaire toxic

## Introduction

Ce projet à pour but de d'utiliser le concept de NLP (natural language processing) qui va nous permettre de juger de la toxicité d'un tweet
> Cette téchnologie peut etre utilisé pour bannir des commentaires inapproprier sur differente plateformes.

Pour cela nous allons utiliser de l'apprentissage supervisé avec `tensorflow` qui va etre notre model de ML mais egalement nous permettre de vecorisé les données ce qui nous sera util lors de l'apprentissage. 

Nous ferons le démploiement sur `gradio`et en "cloud" `huggingface`.


> Les datas ont été recuperer sur `kaggle`et ce présente sous forme de csv: https://www.kaggle.com/datasets/ashwiniyer176/toxic-tweets-dataset?select=FinalBalancedDataset.csv


## DATA
Dans le cadre de notre projet, les datas doivent etre vectorisé mais avant cela il faut tokenisé notre vocabulaire (creer un langage qui sera comprehensible par le model sous forme de valeur numerique).

Une fois tokenisé et notre vocabulaire cree, nous pourrons vectoriser nos tweets.
Il reste une etape final qui consite à préparer le dataset, avant de le donner au model. 
Cette étape prépare le dataset avec une decoupe en lot, d'autres etapes intermédiaire avant de repartir les lots dans les parties train,eval et test.


