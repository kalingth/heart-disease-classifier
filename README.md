# Heart Disease Classifier

Este projeto é um classificador de doença cardíaca que utiliza árvores de decisão para fazer a predição. Ele foi desenvolvido para analisar um conjunto de dados contendo informações sobre pacientes e determinar se o paciente tem ou não doença cardíaca.

## Carga das Bibliotecas e Recuperação dos Dados

O código começa importando as bibliotecas necessárias e carregando os dados de um arquivo CSV disponível em um repositório do GitHub. Em seguida, ele faz uma breve análise dos dados, verificando a existência de linhas duplicadas e dados nulos.

## Funções

O código também inclui algumas funções úteis para realizar análises e treinar os modelos:

- **one_hot_encode_wo_dummies**: Realiza o One-Hot Encoding em atributos categóricos numéricos e remove a coluna original.
- **plot_corr_heatmap**: Plota um mapa de calor para visualizar a correlação entre as variáveis do conjunto de dados.
- **trend_line**: Cria uma linha de tendência para um conjunto de dados bidimensional.
- **cross_val_score**: Realiza validação cruzada usando K-Folds e exibe as métricas de precisão, revocação e acurácia.
- **plot_decision**: Plota o fluxo da tomada de decisão para uma árvore de decisão específica a partir de um dado de entrada.
- **_print_row**: Exibe informações detalhadas sobre a classificação do modelo para uma determinada linha de dados.

## Análise dos Dados

Após a carga dos dados, o código faz uma análise das correlações entre as variáveis usando um mapa de calor. Em seguida, aplica o One-Hot Encoding em algumas variáveis categóricas e plota gráficos de distribuição para visualizar a relação entre algumas variáveis e a variável de saída ("output").

## Treinamento dos Modelos

Em seguida, o código separa as variáveis em conjuntos de treinamento e teste. Ele treina várias árvores de decisão com diferentes configurações e realiza validação cruzada para avaliar o desempenho de cada modelo. Além disso, o código treina um modelo de comitê de decisão (VotingClassifier) que combina as previsões dos modelos individuais.

## Resultados

Após o treinamento, o código exibe as métricas de precisão, revocação e acurácia para cada modelo. Em seguida, ele valida o modelo do comitê de decisão usando um conjunto de teste e mostra a matriz de confusão e o relatório de classificação.

## Auditoria do Modelo

Finalmente, o código realiza uma auditoria do modelo, exibindo o fluxo da tomada de decisão para cada árvore individual no comitê de decisão para um dado de entrada específico.

O projeto fornece uma abordagem detalhada para a construção de um classificador de doença cardíaca usando árvores de decisão e oferece insights sobre a análise dos dados e avaliação do desempenho do modelo. Pode ser usado como base para aprofundamentos em outras áreas de classificação de problemas.
