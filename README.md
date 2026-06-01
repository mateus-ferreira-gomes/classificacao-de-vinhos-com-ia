# 🍷 Wine Quality Analysis and Classification

Projeto desenvolvido na disciplina de **Inteligência Artificial**, com foco em **Análise Exploratória de Dados (EDA)** e **Machine Learning** para classificação de vinhos a partir de suas características químicas.

---

# 📋 Sobre o Projeto

O objetivo deste projeto é analisar dados relacionados à qualidade de vinhos e avaliar o desempenho de diferentes algoritmos de Machine Learning na tarefa de classificação.

O trabalho foi dividido em duas etapas principais:

## 📊 Etapa 1 - Análise Exploratória de Dados (EDA)

Notebook:

📄 `VisualizacaoDados.ipynb`

Atividades realizadas:

- Criação e manipulação de variáveis em Python
- Importação de bibliotecas para análise de dados
- Carregamento do dataset de vinhos
- Verificação de valores nulos
- Identificação de registros duplicados
- Estatísticas descritivas
- Renomeação das colunas para português
- Análise gráfica dos dados
- Exportação do dataset processado

---

## 🤖 Etapa 2 - Machine Learning

Notebook:

📄 `modelos_machine_learning.ipynb`

Atividades realizadas:

- Utilização dos dados preparados na etapa anterior
- Separação entre variáveis preditoras e variável alvo
- Divisão entre treino e teste
- Padronização dos atributos
- Treinamento de modelos de classificação
- Avaliação de desempenho
- Comparação entre algoritmos

---

# 🎯 Problema Investigado

O projeto busca responder à seguinte pergunta:

> É possível utilizar características químicas dos vinhos para classificá-los corretamente por meio de algoritmos de Machine Learning?

Os resultados podem auxiliar na análise da qualidade dos vinhos e apoiar decisões baseadas em dados.

---

# 📊 Base de Dados

Foi utilizado o dataset **Wine Quality Dataset**.

Características da base:

- 6.497 registros
- 13 variáveis
- Dados numéricos e categóricos
- Informações químicas e físicas dos vinhos

## Variáveis analisadas

- Acidez fixa
- Acidez volátil
- Ácido cítrico
- Açúcar residual
- Cloretos
- Dióxido de enxofre livre
- Dióxido de enxofre total
- Densidade
- pH
- Sulfatos
- Álcool
- Qualidade
- Tipo do vinho

---

# 🛠 Tecnologias Utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Google Colab
- Jupyter Notebook

---

# 📈 Análise Exploratória dos Dados

Durante a etapa de EDA foram realizadas as seguintes análises:

## Estatísticas Descritivas

Utilização do método:

```python
df.describe()
```

Obtendo:

- Média
- Desvio padrão
- Valor mínimo
- Valor máximo
- Quartis
- Mediana

## Verificação de Dados

```python
df.isnull().sum()
```

Resultado:

- Nenhum valor nulo encontrado.

```python
df.duplicated().sum()
```

Resultado:

- 1.177 registros duplicados identificados.

## Visualizações Geradas

### Gráfico de Dispersão

- Acidez fixa × Qualidade

### Boxplots

- Qualidade por tipo de vinho
- Teor alcoólico por tipo de vinho

### Heatmap

- Correlação entre variáveis

### Histogramas

- Distribuição das variáveis do dataset

---

# 🤖 Algoritmos Utilizados

## Regressão Logística

Modelo de classificação supervisionada baseado em probabilidades.

Recursos utilizados:

- StandardScaler
- Pipeline
- GridSearchCV
- StratifiedKFold

---

## K-Nearest Neighbors (KNN)

Algoritmo que classifica observações com base nos vizinhos mais próximos.

### Resultado

| Modelo | Acurácia |
|----------|----------|
| KNN | 72% |

---

## Árvore de Decisão

Modelo baseado em regras de decisão.

### Resultado

| Modelo | Acurácia |
|----------|----------|
| Árvore de Decisão | 96% |

---

## Random Forest

Modelo baseado em múltiplas árvores de decisão.

### Resultado

| Modelo | Acurácia |
|----------|----------|
| Random Forest | 100% |

---

# 📊 Comparação dos Resultados

| Algoritmo | Acurácia |
|------------|------------|
| KNN | 72% |
| Árvore de Decisão | 96% |
| Random Forest | 100% |

---

# 📌 Principais Conclusões

- As características químicas dos vinhos possuem forte capacidade preditiva.
- A análise exploratória permitiu compreender melhor a distribuição dos dados.
- Os algoritmos baseados em árvores apresentaram desempenho superior.
- O modelo Random Forest apresentou o melhor resultado, alcançando 100% de acurácia no conjunto de teste.

---


# 👨‍🎓 Autor

**Mateus Ferreira Gomes**

Disciplina: **Inteligência Artificial**

Ano: **2026**
