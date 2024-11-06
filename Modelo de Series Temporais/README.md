# Modelo de Series Temporais | Machine Learning

## Introdução

No meu projeto, utilizei um modelo de machine learning para prever as vendas de um departamento com bases em datas sazonais de feriados, para descobruir qual será o desempenho das vendas, utilizando um modelo de series temporais.

__Link da base no Kaggle:__ https://www.kaggle.com/code/ssathishkumar/retail-sales-forecasting-time-series-eda/notebook


<details>
<summary>Dicionário de Dados</summary>

- **Store**: Número identificador da loja (tipo inteiro).
- **Dept**: Número identificador do departamento (tipo inteiro).
- **Date**: Data de registro das vendas (tipo texto, object).
- **Weekly_Sales**: Pressão arterial em repouso (em mm Hg).
- **IsHoliday**: Indicador de feriado (tipo bool).

</details>


## Metricas utilizadas


Acurácia<br>
Taxa de erro<br>


Gráficos de PLOT para visualização.


## Algoritmo utilizado

**SARIMA**

É um algoritmo de séries temporais que amplia o modelo ARIMA para lidar com dados que apresentam sazonalidade, ou seja, padrões que se repetem em intervalos regulares, como dias, semanas, meses ou anos.


O SARIMA é definido por dois conjuntos de parâmetros:

Parâmetros Não Sazonais (p, d, q):
p: Número de defasagens (lags) no componente autoregressivo (AR).
d: Número de diferenciações aplicadas para tornar a série estacionária.
q: Número de defasagens no componente de média móvel (MA).
Parâmetros Sazonais (P, D, Q, s):
P: Número de defasagens para o componente autoregressivo sazonal.
D: Número de diferenciações sazonais para remover sazonalidade.
Q: Número de defasagens para o componente de média móvel sazonal.
s: Período sazonal, indicando a frequência do ciclo sazonal (por exemplo, 12 para dados mensais com sazonalidade anual).


--------

## Modelos Machine Learning </>




<details> <summary> Modelo </summary>

## Desenvolvimento


Neste projeto, utilizei técnicas de machine learning para desenvolver um modelo capaz de prever o desempenho das vendas de uma loja específica com o proximo periodo. O desenvolvimento seguiu os seguintes passos:

**Exploração e Análise dos Dados:**
A base de dados foi carregada e explorada para entender melhor suas características. Verifiquei a distribuição de valores, identifiquei possíveis valores ausentes e analisei a correlação entre os atributos.

Arquivo: sales_dataset
Modelo: serial_temp_sales