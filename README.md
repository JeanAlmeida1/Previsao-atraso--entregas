# Modelo de classificação: previsao de atraso de entregas.

Criação de um modelo com o objetivo de prever quais entregas atrasarão, desenvolvido para o Hackathon da DNC powered by UELLO.

A maior dificuldade na criação do modelo foi a pouca quantidade de features, o que tornou necessário a elaboração de novas variáveis, incluindo a utilização de um algoritmo de clusterização (DBScan) para agrupar cidades semelhantes.

Após vários testes, o modelo final escolhido para realizar as previsões foi um Random Forest com otimização de hiperparâmetros via GridSearchCV, por ter apresentado métricas satisfatórias - principalmente f1 score - nos dados de teste. 

Passo a passo realizado:

	* Inspeção inicial dos dados
	* Análise descritiva
	* Criação de variável target de atraso
	* Criação de variável de complexidade do pedido
	* Transformação de variáveis: one hot encoding e transformação de tipos 
	* Clusterização de cidades: escolha e execução do melhor algoritmo 
	* Criação do dataframe final com as variáveis transformadas	
	* Divisão de dados entre treino e teste
	* Classificação: escolha e execução do melhor algoritmo
	* Análise de multicolinearidade (VIF) 
	* Otimização de hiperparâmetros via GridSearchCV 
  
