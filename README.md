Análise de Churn de Clientes - Telecom X

Este projeto em Python realiza uma análise exploratória de dados (EDA) para identificar os principais fatores que levam clientes da Telecom X a cancelar seus serviços (churn). O objetivo é fornecer insights claros e acionáveis para desenvolver estratégias eficazes de retenção de clientes.

Clique duas vezes (ou pressione "Enter") para editar

⚙️ Funcionalidades
1. Pré-processamento e Limpeza de Dados :
Normalização de Dados: Transformação de dados JSON para um formato tabular (DataFrame pandas).
Tratamento de Valores Ausentes: Identificação e remoção de linhas com dados inconsistentes, especialmente na variável alvo Churn e faturamento.
Ajuste de Tipos de Dados: Conversão de colunas para os tipos apropriados (float, int, etc.).
Engenharia de Features: Criação de novas variáveis, como Contas_Diarias, para enriquecer a análise.
adronização e Tradução: Renomeação de colunas e tradução de categorias (gênero, tipo_contrato, método_pagamento) para facilitar a interpretação.
2. Análise Exploratória de Dados (EDA)
Perfil do Cliente que Cancela: Identificação das características demográficas e de serviço mais comuns em clientes que efetuam churn.
Impacto do Tipo de Contrato: Análise da relação entre a duração do contrato (mensal, anual, bienal) e a taxa de churn.
Serviços de Internet e Churn: Investigação de como o tipo de serviço de internet (DSL, Fibra Óptica, ou sem serviço) influencia a decisão de cancelar.
Métodos de Pagamento e Churn: Avaliação da correlação entre os diferentes métodos de pagamento e a propensão ao churn.
Correlações entre Variáveis: Exploração das relações entre as diversas características do cliente (tempo de contrato, faturamento, serviços adicionais) e a variável
🚀 Como Utilizar
Dados de Entrada
O projeto espera que os dados sejam fornecidos a partir de uma URL no formato JSON. O notebook já configura a requisição para https://raw.githubusercontent.com/alura-cursos/challenge2-data-science/main/TelecomX_Data.json.

Bibliotecas Necessárias
Certifique-se de ter as seguintes bibliotecas Python instaladas:

pandas para manipulação de dados.
numpy para operações numéricas.
matplotlib.pyplot para visualizações gráficas básicas.
seaborn para visualizações estatísticas aprimoradas.
plotly.express para gráficos interativos.
requests para fazer requisições HTTP e obter os dados.
Você pode instalá-las via pip: pip install pandas numpy matplotlib seaborn plotly requests

Execução do Programa
Abra o notebook Jupyter (ou Google Colab) AluraETF.ipynb.
Execute todas as células do notebook sequencialmente. O programa fará o download dos dados, realizará o pré-processamento e exibirá as análises exploratórias.*
🔍 Análise dos Resultados
Após a execução do notebook, observe os seguintes resultados e insights:

Taxa Geral de Churn: A distribuição inicial de clientes que cancelam ou permanecem. Este é o ponto de partida para entender a dimensão do problema.

Gráficos de Distribuição por Categorias

Gênero, Idoso, Dependentes: Observe se há diferenças significativas na taxa de churn entre esses grupos. No caso, idosos e clientes sem dependentes mostraram maior propensão.
Tipo de Contrato: Verifique qual modalidade de contrato (mensal, anual, bienal) possui a maior taxa de evasão, o que sugere um ponto crítico para intervenção.
Serviço de Internet: Analise se um tipo específico de conexão (e.g., Fibra Óptica) tem um churn mais alto, indicando possíveis problemas de qualidade ou precificação.
Método de Pagamento: Identifique se algum método de pagamento específico está associado a maior churn.
Matriz de Correlação: Analise a relação entre as variáveis e o cancelou_servico. Correlações mais fortes (positivas ou negativas) indicam maior influência no churn. Por exemplo, meses_contrato com correlação negativa (quanto mais tempo, menos churn) e Contas_Diarias com correlação positiva (contas diárias elevadas, maior churn).

A partir dessa análise, será possível identificar os principais gatilhos de churn e direcionar esforços para retenção de forma mais eficaz
