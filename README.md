# Projeto - Desgaste de Pastilha de Freio

Neste projeto, abordamos um problema real da indústria rodoviária: a previsão da quilometragem restante até a troca das pastilhas de freio. O desgaste das pastilhas é crucial para a segurança dos veículos, e prever quando a troca é necessária pode ajudar na manutenção preventiva, reduzindo custos e aumentando a segurança.

Começamos importando as bibliotecas necessárias, como `numpy`, `pandas`, `matplotlib` e `seaborn`, para manipulação de dados e visualização. Em seguida, carregamos o dataset a partir de um arquivo CSV, realizando ajustes para garantir que os dados numéricos fossem interpretados corretamente.

Após a preparação dos dados, realizamos uma análise exploratória, que incluiu um resumo estatístico e a verificação de valores ausentes. Isso nos permitiu entender a distribuição dos dados e identificar potenciais problemas de qualidade.

Um passo fundamental foi o cálculo das variações de desgaste para cada roda e a determinação dos coeficientes de desgaste correspondentes. Esses coeficientes são essenciais para prever a quilometragem restante, já que representam a relação entre desgaste e quilometragem.

A matriz de correlação foi gerada para analisar as relações entre as variáveis do dataset. Essa análise nos ajudou a identificar quais variáveis estavam mais fortemente relacionadas e poderiam ser usadas na modelagem.

Optamos pela **Ridge Regression** como modelo principal, pois demonstrou um desempenho superior nas métricas de avaliação, como RMSE e MAE. Para melhorar ainda mais a precisão das previsões, aplicamos a **transformação logarítmica** nas variáveis de desgaste. Essa transformação ajudou a linearizar as relações entre as variáveis, permitindo que o modelo se ajustasse melhor aos dados e resultando em previsões mais confiáveis.

Finalmente, implementamos uma interface interativa que permite aos usuários inserir dados de desgaste e obter previsões sobre a quilometragem restante até a troca das pastilhas de freio. Essa funcionalidade torna o modelo aplicável e útil na prática, beneficiando os usuários da indústria rodoviária.

Em resumo, nosso código foi desenvolvido de forma sistemática para resolver o problema do desgaste das pastilhas de freio, desde a coleta e análise de dados até a implementação de uma interface interativa. Essa abordagem não apenas melhorou a compreensão dos dados, mas também resultou em um modelo preditivo prático e eficaz, ajudando a aumentar a segurança e a eficiência na manutenção de veículos.
