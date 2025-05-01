# Estimativa de Faturamento para Expansão de Negócios

Este projeto tem como objetivo estimar o potencial de faturamento em bairros de São Paulo para uma empresa alimentícia situada no Rio de Janeiro, que deseja expandir suas operações. A análise utiliza dados sociodemográficos e de faturamento dos bairros do Rio de Janeiro como base para prever o faturamento em São Paulo.

## Estrutura do Projeto

### Arquivos

- **`prediction_invoicing.ipynb`**: Notebook contendo a análise exploratória, preparação dos dados, treinamento de modelos de previsão e avaliação dos resultados.
- **`data/dados.csv`**: Arquivo CSV com dados sociodemográficos e de faturamento dos bairros do Rio de Janeiro e São Paulo.
- **`data/descritivo_dados.pdf`**: Documento descritivo com informações detalhadas sobre os dados disponíveis.

## Objetivos

1. **Análise exploratória e preparação dos dados**:
   - Filtrar os dados para o público-alvo: adultos de 25 a 50 anos das classes A (rendas A1 e A2) e B (rendas B1 e B2).
   - Tratar valores nulos e ajustar colunas relevantes.

2. **Treinamento de modelos preditivos**:
   - Modelos utilizados:
     - Regressão Linear
     - Random Forest
     - Gradient Boosting
   - Avaliação dos modelos com métricas como MSE (Erro Quadrático Médio) e R² (Coeficiente de Determinação).

3. **Validação e comparação dos modelos**:
   - Comparar os resultados dos modelos para selecionar o mais adequado.

## Resultados

### Modelos Treinados

- **Random Forest**:
  - Melhor desempenho com R² de 0.8775.
  - Valores preditos bem alinhados com os valores reais.
- **Gradient Boosting**:
  - R² de 0.8439, desempenho próximo ao Random Forest.
- **Regressão Linear**:
  - Menor desempenho com R² de 0.8195.

### Conclusão

O modelo de Random Forest foi escolhido como o mais adequado para prever o faturamento nos bairros de São Paulo. No entanto, o Gradient Boosting também apresentou resultados satisfatórios. A inclusão de variáveis adicionais pode melhorar ainda mais a precisão das previsões.
