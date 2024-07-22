# Projeto: Interconnect Telecom

## Plano de Trabalho para a conclusão do projeto

**ETAPA 1: PLANEJAMENTO**

1. Definição do objetivo:

    - Prever a rotatividade dos clientes da Interconnect
    - Métrica Primária: AUC-ROC
    - Métrica Secundária: Acurácia.

2. Coleta de dados:

    - Baixar e inspencionar os arquivos: contract.csv, personal.csv, internet.csv e phone.csv
    - Verificar se todos os arquivos contêm a coluna "customerID".

**ETAPA 2: INVESTIGAÇÃO DOS DADOS**

1. Análise Exploratória dos Dados (EDA):

    - Importar as bibliotecas necessárias para a tarefa
    - Carregar os dados dos arquivos
    - Verificar tipo de dados, valores ausentes e distribuição das variáveis
    - Utilizar gráficos para melhor entendimento dos dados

2. Pré-processamento de Dados:

    - Tratamento de valores ausentes
    - Ver a necessidade de balanceamento dos dados
    - Codificação das variáveis categóricas
    - Normalizar ou padronizar variáveis numéricas, se necessário

**ETAPA 3: DESENVOLVIMENTO DO MODELO**

1. Divisão dos dados:

    - Dividir os dados em conjunto de treino, teste e validação

2. Seleção de Modelos:

    - Escolher modelos de Machine Learning para resolver um problema de Classificação, na variável alvo `EndDate`, como por exemplo: Regressão Logística, DecisionTreeClassifier, RandomForestClassifier, GBM, SVM e outros.

3. Treinamento de Modelos:

    - Treinar diferentes modelos nos dados de treino

4. Avaliação do modelo:

    - Avaliar modelos utilizando a métrica AUC-ROC
    - Selecionar modelos com melhores desempenhos

5. Ajuste de Hiperparâmetros:

    - Realizar a otimização de hiperparâmetros, utilizando o GridSearch

6. Validação Cruzada:

    - Utilizar validação cruzada para assegurar a robustez do modelo.

**ETAPA 4: PREPARAÇÃO DO RELATÓRIO**

1. Resultados

    - Desempenho dos modelos testados com foco na métrica AUC-ROC e na acurácia.
    - Tabela e gráficos comparativos dos modelos.

2. Conclusão e Recomendações:

    - Conclusões baseadas nos resultados.
    - Recomendações para a Interconnect sobre como utilizar o modelo para reduzir a rotatividade.

---
