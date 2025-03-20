# Classificacao_por_tras_dos_panos
O projeto que desenvolvi consistiu em uma análise de dados de uma empresa que buscava identificar potenciais clientes propensos a deixar seus serviços ou churn. O objetivo era, por meio de modelos de machine learning, prever quais clientes estavam em risco de sair de nossa empresa, permitindo que a companhia tomasse ações preventivas para reter esses clientes.

Para realizar a análise, utilizei Pandas e NumPy como ferramentas principais para manipulação e processamento dos dados. O Pandas foi fundamental para a organização e limpeza dos dados. O NumPy foi utilizado para realizar os cálculos numéricos.

Utilizei três modelos de classificação distintos: KNN (K-Nearest Neighbors), Bernoulli Naive Bayes e Árvore de Decisão. 

KNN (K-Nearest Neighbors): Neste modelo, usei a métrica do cálculo da distância euclidiana entre as observações para determinar quais clientes são mais semelhantes entre si.

Bernoulli Naive Bayes: Aqui, adotei o processo de binarização das variáveis de entrada, utilizando a mediana das colunas de X para transformar os dados em um formato binário. Ideal para o uso nesse caso por conta que as variáveis binárias, como no caso do churn.

Árvore de Decisão: No modelo de árvore de decisão, utilizei o critério de entropia para a divisão dos dados. Esse critério permite construir árvores de decisão que maximizam a informação obtida em cada divisão, e o obteve um melhor resultado em relação ao índice de gini

Para garantir a validação adequada dos modelos, utilizei a técnica de train_test_split, que separa os dados em conjuntos de treino e teste.

Na fase de avaliação, utilizei três métricas de desempenho: accuracy score, precision score e recall score. Para este caso específico, a métrica mais relevante foi o recall score, já que o principal objetivo era identificar de forma eficaz os clientes com maior risco de churn. O recall score ajuda a medir a capacidade do modelo em identificar corretamente os casos positivos (clientes com risco de churn).
