# 📝 Sobre o Dataset

Este projeto consiste na análise e construção de um modelo preditivo baseado em dados oficiais da Polícia Rodoviária Federal (PRF / DENATRAN), retirados do https://dados.gov.br .

## Objetivo Principal / Variável Alvo: 
Foi definida como variável-alvo a `classificacao_acidente`, visando prever a gravidade da ocorrência entre três classes: Com Vítimas Feridas, Sem Vítimas e Com Vítimas Fatais.

## Tratamento dos Dados: 
Remoção de dados nulos e exclusão de colunas redundantes ou com vazamento de dados (data leakage, como contagem de mortos e feridos).

## Modelagem: 
Implementação de um Pipeline no Scikit-Learn utilizando StandardScaler para dados numéricos, OneHotEncoder para categóricos e o algoritmo RandomForestClassifier.

## Resultados: 
Otimização via RandomizedSearchCV, alcançando uma acurácia final de 79,69% no conjunto de teste.
