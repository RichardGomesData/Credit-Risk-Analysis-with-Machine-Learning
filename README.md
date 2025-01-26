# Credit Risk Analysis with Machine Learning
 Credit Risk Analysis with Machine Learning



## 1. Coleta de Dados
Os dados utilizados neste projeto foram coletados de um repositório público no GitHub. O dataset contém informações sobre clientes, incluindo dados financeiros, características pessoais e comportamento relacionado ao uso de cartão de crédito.

**Fonte dos Dados**:  
[Dataset de crédito](https://raw.githubusercontent.com/andre-marcos-perez/ebac-course-utils/main/dataset/credito.csv)

Os dados foram processados para corrigir inconsistências, como transformar valores de salário anual, limite de crédito e transações em formato numérico e tratar valores ausentes.

---

## 2. Modelagem
Foi desenvolvido um modelo de classificação para prever a variável `default` (inadimplência). O pipeline incluiu os seguintes passos:

1. **Pré-processamento**:
   - Conversão de variáveis categóricas em variáveis dummy.
   - Separação dos dados em conjunto de treino (80%) e teste (20%).

2. **Modelo Utilizado**:
   - **Random Forest Classifier**:
     - Hiperparâmetros padrão.
     - Utilizado devido à sua robustez e bom desempenho em problemas de classificação.

3. **Métricas de Avaliação**:
   - Relatório de classificação (`precision`, `recall`, `f1-score`).
   - Matriz de confusão.
   - AUC-ROC (Área Sob a Curva ROC).

**Resultados do Modelo**:
- **Acurácia**: 93%
- **AUC-ROC**: 0.967  
O modelo apresentou bom desempenho, com alta precisão e recall para a classe majoritária e valores satisfatórios para a classe minoritária.

---

## 3. Visualização dos Dados
Durante a análise exploratória, foram gerados diversos gráficos para entender os padrões do dataset:

- **Distribuição do Salário Anual**: Histograma e boxplot.
- **Correlação entre Variáveis**: Heatmap de correlação.
- **Relação entre Escolaridade e Salário**: Boxplot.
- **Relação entre Meses de Relacionamento e Salário**: Linha de tendência.

Para os resultados do modelo, seria interessante incluir gráficos como:
- **Matriz de Confusão**: Representação gráfica do desempenho do modelo.
- **Curva ROC**: Visualização do desempenho geral do modelo.

---

## 4. Conclusões
O trabalho atendeu ao objetivo de construir e avaliar um modelo preditivo para inadimplência utilizando técnicas de aprendizado de máquina. O modelo Random Forest apresentou resultados robustos, sendo adequado para prever a variável `default`.

**Limitações e Próximos Passos**:
- **Imbalance**: A classe `default` (inadimplente) está desbalanceada. Técnicas como oversampling (SMOTE) podem ser exploradas.
- **Tuning do Modelo**: Ajuste de hiperparâmetros do Random Forest para melhorar ainda mais o desempenho.
- **Expansão das Visualizações**: Incluir gráficos como a curva ROC e matriz de confusão.

---

## 5. Repositório GitHub
Os códigos, dados e visualizações estão disponíveis no repositório GitHub:  
[Link para o Repositório](#)

---

**Autor**: Richard Gomes  
**Ferramentas Utilizadas**: Python, Pandas, Seaborn, Scikit-learn, Matplotlib
