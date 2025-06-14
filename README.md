
# 🏠 House Prices: Regressão com Modelos de Machine Learning

Este projeto utiliza técnicas de aprendizado de máquina supervisionado para prever o preço de venda de imóveis, com base em dados estruturados de um dataset da competição *House Prices - Advanced Regression Techniques* (Kaggle). Foram aplicados modelos como **Regressão Linear**, **Árvore de Decisão** e **KNN Regressor**, com comparação de desempenho entre eles.

## 📁 Arquivos

- `train.csv`: dados de treino com os preços reais dos imóveis.
- `test.csv`: dados de teste onde os preços devem ser previstos.
- `resultado.csv`: arquivo gerado com as previsões finais da Regressão Linear.
- `house.py`: script principal com todo o pipeline de processamento, treino, teste e exportação de resultados.

## 🚀 Tecnologias Utilizadas

- Python 3
- Pandas
- Scikit-learn
- Matplotlib

## ⚙️ Etapas do Projeto

1. **Carregamento e análise inicial dos dados**
2. **Limpeza dos dados**:
   - Remoção de colunas com mais de 10% de valores nulos
   - Preenchimento de valores faltantes com -1
   - Seleção apenas das colunas numéricas
3. **Separação entre atributos (X) e target (y)**
4. **Treinamento dos modelos**:
   - Linear Regression
   - Decision Tree Regressor
   - KNN Regressor (K=2)
5. **Avaliação com métricas**:
   - MAE (Erro Absoluto Médio)
   - MSE (Erro Quadrático Médio)
6. **Visualização gráfica das previsões x valores reais**
7. **Previsão dos dados de teste e exportação para CSV**

## 📊 Resultado

O projeto compara a performance dos modelos em termos de erro e exibe visualmente o quão próximas estão as previsões dos valores reais. O modelo que gera o `resultado.csv` é o de **Regressão Linear**, devido à sua melhor generalização nos testes.

## ▶️ Como Executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/nome-do-repositorio.git
   cd nome-do-repositorio
   ```
2. Instale os pacotes necessários:
   ```bash
   pip install pandas scikit-learn matplotlib
   ```
3. Execute o script:
   ```bash
   python modelo.py
   ```
4. O arquivo `resultado.csv` será gerado com as previsões.

## 📝 Observações

- Apenas colunas numéricas foram utilizadas no modelo.
- O preenchimento com `-1` é uma técnica simples e pode ser melhorada com engenharia de atributos futura.
- O valor de K (2) no KNN foi escolhido de forma empírica.
