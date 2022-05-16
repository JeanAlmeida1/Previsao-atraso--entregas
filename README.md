# Modelo de classificação: previsao de atraso de entregas.

Criação de um modelo com o objetivo de prever quais entregas atrasarão, desenvolvido para o Hackathon da DNC powered by UELLO.

A maior dificuldade na criação do modelo foi a pouca quantidade de features, o que tornou necessário a elaboração de novas variáveis, incluindo a utilização de um algoritmo de clusterização (DBScan) para agrupar cidades semelhantes.

Após vários testes, o modelo final escolhido para realizar as previsões foi um Random Forest com otimização de hiperparâmetros via GridSearchCV, por ter apresentado métricas satisfatórias - principalmente f1 score - nos dados de teste. 
