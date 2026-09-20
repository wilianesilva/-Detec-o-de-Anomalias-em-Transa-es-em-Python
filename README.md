#  Detecção de Anomalias em Transações Financeiras

Este projeto tem como objetivo desenvolver e avaliar um modelo de **Machine Learning** capaz de identificar transações fraudulentas (anômalas) em dados de cartão de crédito.

O principal desafio deste problema é o alto desbalanceamento das classes, uma vez que transações legítimas representam a esmagadora maioria das operações, enquanto as fraudes correspondem a uma fração muito pequena dos eventos.

---

##  Etapas do Projeto

1. **Análise Exploratória dos Dados (EDA):** Carregamento do dataset e verificação da distribuição das variáveis e das classes normais vs. anômalas.
2. **Pré-processamento:** Normalização de variáveis numéricas (`Amount`) e divisão dos dados em conjuntos de treino e teste mantendo a proporção das classes com `stratify`.
3. **Tratamento de Desbalanceamento:** Aplicação da técnica de oversampling **SMOTE** (*Synthetic Minority Over-sampling Technique*) na base de treino para equilibrar a representatividade das classes.
4. **Treinamento do Modelo:** Utilização do algoritmo **Random Forest Classifier** para aprender os padrões das transações.
5. **Avaliação de Desempenho:** Análise focada em métricas adequadas para dados desbalanceados (**Precision**, **Recall**, **F1-Score** e **ROC-AUC**).
6. **Explicabilidade:** Identificação das variáveis de maior relevância para o diagnóstico de anomalias.

---

##  Tecnologias e Bibliotecas Utilizadas

* **Linguagem:** Python 3
* **Manipulação de Dados:** Pandas, NumPy
* **Visualização de Dados:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-Learn
* **Tratamento de Desbalanceamento:** Imbalanced-Learn (`imblearn`)

---

##  Resultados e Métricas

* **ROC-AUC Score:** Avalia a capacidade geral do modelo de distinguir entre transações legítimas e fraudulentas.
* **Recall:** Garante que a maior quantidade possível de fraudes reais seja detectada (reduzindo falsos negativos).
* **Precision:** Mede a acurácia das alertas de fraude emitidos pelo modelo (reduzindo falsos positivos).

