# (EN) # Energy Demand Forecasting - Time Series Analysis

## Introduction

This project focuses on a comparative analysis between ARIMA (Autoregressive Integrated Moving Average) models and Recurrent Neural Networks (RNNs) for forecasting electricity demand in Brazil. Accurate energy demand prediction is crucial for efficient and sustainable planning in the energy sector, contributing to resource optimization, overload prevention, and waste reduction.

In the Brazilian context, where the energy matrix is one of the cleanest in the world with significant participation of renewable sources, the importance of this study is even more pronounced. According to recent data, renewable sources will represent a significant portion of the installed capacity for electricity generation in Brazil in the coming years.

![Brazilian Energy Matrix](img/matriz_energetica.png)

Accurate demand forecasting is fundamental for the success of government initiatives and long-term planning of the energy sector, contributing to a more sustainable, economical, and equitable energy development for the Brazilian population.

## Objectives

The main objective of this work is to forecast electricity demand in Brazil, using and comparing two robust methods: the ARIMA model and RNNs. The specific objectives include:

1. Exploratory analysis of energy demand data
2. Implementation and adjustment of ARIMA and RNN models
3. Comparison of model performance using the MAPE (Mean Absolute Percentage Error) metric
4. Identification of the most effective method considering accuracy, complexity, and applicability to real data

## Methodology

1. **Exploratory Data Analysis**: Identification of trends, seasonalities, and possible outliers in the energy demand time series.

![Exploratory Analysis](img/analise_exploratoria.png)

2. **Model Implementation**:
   - ARIMA: Model adjustment to capture trends and seasonal patterns
   - RNN: Utilization of GRU (Gated Recurrent Unit) architecture with hyperparameter tuning

3. **Performance Evaluation**: Use of MAPE (Mean Absolute Percentage Error) metric to compare model accuracy

## Results

### ARIMA Model

- MAPE: 1.97% (98.03% accuracy)
- Excellent capability to capture trends and seasonal patterns
- Processing time: between 1.5 to 2 hours

![ARIMA Results](img/resultados_arima.png)

### RNN Model (GRU)

- MAPE: 4.11% (95.89% accuracy)
- Significantly higher computational efficiency than ARIMA
- Best performance with 2 years of validation data (MAPE of 4.16%)

![RNN Results](img/resultados_rnn.png)

## Conclusions

1. The ARIMA model showed slightly superior accuracy (MAPE of 1.97%) but with high computational cost.
2. The RNN model, although less accurate (MAPE of 4.11%), proved to be remarkably efficient in computational terms, making it more suitable for applications requiring frequent updates or real-time processing.
3. The choice between models should consider not only accuracy but also complexity and execution time, depending on the specific needs of the application.

The analysis of variation in validation and test years provided additional information about the behavior of the models. The RNN, for example, showed better performance with 2 years of validation, achieving a MAPE of 4.16%.

![Model Comparison](img/comparacao_modelos.png)

## Implications and Contributions

- Optimization of energy generation and distribution, potentially reducing operational costs and tariffs for consumers.
- Contribution to the efficient integration of renewable energy sources, promoting a cleaner and more sustainable energy matrix.
- Provision of practical and theoretical insights for applying advanced time series modeling techniques in the context of the Brazilian electricity sector.

## Future Perspectives

- Incorporation of exogenous variables in the models
- Exploration of more advanced architectures, such as Transformers
- Development of models capable of providing probabilistic forecasts

This study demonstrates the significant potential of advanced time series modeling techniques in forecasting electricity demand. The successful application of these models can substantially contribute to a more efficient, economical, and sustainable energy sector in Brazil, aligning with the country's sustainable development goals and energy transition targets.

# (PT-BR) # Previsão de Demanda de Energia - Análise de Séries Temporais

## Introdução

Este projeto concentra-se na análise comparativa entre os modelos ARIMA (Autoregressive Integrated Moving Average) e Redes Neurais Recorrentes (RNNs) para a previsão da demanda de energia elétrica no Brasil. A previsão precisa da demanda energética é crucial para o planejamento eficiente e sustentável do setor, contribuindo para a otimização do uso de recursos, prevenção de sobrecargas e redução de desperdícios.

No contexto brasileiro, onde a matriz energética é uma das mais limpas do mundo, com significativa participação de fontes renováveis, a importância deste estudo é ainda mais pronunciada. Segundo dados recentes, as fontes renováveis representarão uma parcela expressiva da capacidade instalada de geração de energia elétrica no Brasil nos próximos anos.

![Matriz Energética Brasileira](img/matriz_energetica.png)

A previsão acurada da demanda é fundamental para o sucesso de iniciativas governamentais e para o planejamento a longo prazo do setor energético, contribuindo para um desenvolvimento energético mais sustentável, econômico e equitativo para a população brasileira.

## Objetivos

O objetivo principal deste trabalho é realizar a previsão da demanda de energia elétrica no Brasil, utilizando e comparando dois métodos robustos: o modelo ARIMA e as RNNs. Os objetivos específicos incluem:

1. Análise exploratória dos dados de demanda energética
2. Implementação e ajuste dos modelos ARIMA e RNN
3. Comparação da performance dos modelos utilizando a métrica MAPE (Mean Absolute Percentage Error)
4. Identificação do método mais eficaz considerando precisão, complexidade e aplicabilidade em dados reais

## Metodologia

1. **Análise Exploratória dos Dados**: Identificação de tendências, sazonalidades e possíveis outliers na série temporal de demanda energética.

![Análise Exploratória](img/analise_exploratoria.png)

2. **Implementação dos Modelos**:
   - ARIMA: Ajuste do modelo para capturar tendências e padrões sazonais
   - RNN: Utilização da arquitetura GRU (Gated Recurrent Unit) com ajuste de hiperparâmetros

3. **Avaliação de Desempenho**: Utilização da métrica MAPE (Mean Absolute Percentage Error) para comparar a precisão dos modelos

## Resultados

### Modelo ARIMA

- MAPE: 1,97% (precisão de 98,03%)
- Excelente capacidade de capturar tendências e padrões sazonais
- Tempo de processamento: entre 1h30 e 2 horas

![Resultados ARIMA](img/resultados_arima.png)

### Modelo RNN (GRU)

- MAPE: 4,11% (precisão de 95,89%)
- Eficiência computacional significativamente maior que o ARIMA
- Melhor desempenho com 2 anos de validação (MAPE de 4,16%)

![Resultados RNN](img/resultados_rnn.png)

## Conclusões

1. O modelo ARIMA apresentou precisão ligeiramente superior (MAPE de 1,97%), mas com alto custo computacional.
2. O modelo RNN, embora menos preciso (MAPE de 4,11%), mostrou-se notavelmente eficiente em termos computacionais, tornando-o mais adequado para aplicações que requerem atualizações frequentes ou processamento em tempo real.
3. A escolha entre os modelos deve considerar não apenas a precisão, mas também a complexidade e o tempo de execução, dependendo das necessidades específicas da aplicação.

A análise da variação dos anos de validação e teste forneceu informações adicionais sobre o comportamento dos modelos. O RNN, por exemplo, apresentou melhor desempenho com 2 anos de validação, atingindo um MAPE de 4,16%.

![Comparação de Modelos](img/comparacao_modelos.png)

## Implicações e Contribuições

- Otimização da geração e distribuição de energia, potencialmente reduzindo custos operacionais e tarifas para os consumidores.
- Contribuição para a integração eficiente de fontes de energia renováveis, promovendo uma matriz energética mais limpa e sustentável.
- Fornecimento de insights práticos e teóricos para a aplicação de técnicas avançadas de modelagem em séries temporais no contexto do setor elétrico brasileiro.

## Perspectivas Futuras

- Incorporação de variáveis exógenas nos modelos
- Exploração de arquiteturas mais avançadas, como Transformers
- Desenvolvimento de modelos capazes de fornecer previsões probabilísticas

Este estudo demonstra o potencial significativo das técnicas avançadas de modelagem de séries temporais na previsão da demanda de energia elétrica. A aplicação bem-sucedida desses modelos pode contribuir substancialmente para um setor energético mais eficiente, econômico e sustentável no Brasil, alinhando-se com os objetivos de desenvolvimento sustentável e as metas de transição energética do país.
