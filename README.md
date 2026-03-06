# 📊 Análise de Dados do Campeonato Brasileiro

## 📌 Descrição do Projeto

Este projeto tem como objetivo realizar uma **análise exploratória inicial de dados (EDA)** utilizando Python a partir de um dataset contendo informações sobre partidas do **Campeonato Brasileiro**.

O script realiza operações básicas de **leitura, inspeção e exploração de dados**, permitindo compreender a estrutura do dataset e preparar as informações para futuras análises e visualizações.

Além disso, o projeto foi estruturado pensando em **expansão futura para ferramentas de Business Intelligence**, como **Power BI**, permitindo a criação de dashboards e relatórios interativos.

---

## 🛠️ Tecnologias Utilizadas

* **Python 3**
* **Pandas** → Manipulação e análise de dados
* **NumPy** → Operações numéricas
* **Matplotlib** → Visualização de dados
* **CSV Dataset** → Base de dados do campeonato brasileiro

Bibliotecas utilizadas no código:

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
```

---

## 📂 Estrutura do Projeto

```
Dados_Campeonato/
│
├── DadosCampeonato.py
├── campeonato_brasileiro_full.csv
└── README.md
```

---

## 📥 Fonte dos Dados

O dataset utilizado contém informações sobre jogos do **Campeonato Brasileiro**, incluindo:

* Time mandante
* Time visitante
* Resultados
* Informações das partidas
* Estatísticas relacionadas aos jogos

Arquivo utilizado:

```
campeonato_brasileiro_full.csv
```

---

## ⚙️ Funcionalidades do Script

O script realiza as seguintes operações:

### 📖 1. Leitura do Dataset

```python
Dados = pd.read_csv('c:/Users/olive/Desktop/Dados_Campeonato/campeonato_brasileiro_full.csv', sep=',')
```

Carrega o dataset em um **DataFrame do Pandas**.

---

### 🔎 2. Visualização inicial dos dados

```python
print(Dados.head())
```

Exibe as **primeiras linhas do dataset** para entender sua estrutura.

---

### 🏟️ 3. Seleção de Colunas

```python
print(Dados['mandante'])
```

Seleciona e exibe a coluna **mandante**, contendo os times que jogaram como mandantes.

---

### 📊 4. Acesso a linhas específicas

```python
Dados.iloc[1]
```

Permite acessar uma linha específica do dataset.

---

### 🧾 5. Informações estruturais do DataFrame

```python
Dados.info()
```

Exibe:

* número de colunas
* tipos de dados
* valores nulos
* estrutura geral do dataset

---

### 📐 6. Dimensão do Dataset

```python
Dados.shape
```

Mostra:

* número de **linhas**
* número de **colunas**

---

### 📄 7. Exibição completa dos dados

```python
print(Dados)
```

Mostra todo o DataFrame carregado.

---

## 📊 Possíveis Expansões do Projeto

Este projeto pode evoluir para análises mais avançadas, como:

* 📈 Número de vitórias por time
* 🏆 Times com melhor desempenho como mandante
* ⚽ Média de gols por rodada
* 📅 Evolução de desempenho ao longo das temporadas
* 📊 Visualizações gráficas com **Matplotlib ou Seaborn**

Exemplo de gráfico futuro:

```python
Dados['mandante'].value_counts().plot(kind='bar')
plt.show()
```

---

## 📊 Integração com Power BI

O dataset pode ser utilizado em ferramentas de **Business Intelligence**, como o **Power BI**, para criar dashboards interativos.

Possibilidades de análise no Power BI:

* Ranking de times
* Performance por temporada
* Comparação mandante vs visitante
* Distribuição de resultados
* Estatísticas de partidas

Fluxo possível de integração:

```
Dataset CSV
      ↓
Python (limpeza e tratamento)
      ↓
Exportação para CSV ou Banco de Dados
      ↓
Power BI
      ↓
Dashboard interativo
```

---

## 🚀 Como Executar o Projeto

1️⃣ Instale as bibliotecas necessárias

```bash
pip install pandas numpy matplotlib
```

2️⃣ Execute o script

```bash
python DadosCampeonato.py
```

---

## 🎯 Objetivo do Projeto

Este projeto faz parte de um processo de aprendizado em:

* **Análise de Dados**
* **Manipulação de dados com Python**
* **Exploração de datasets esportivos**
* **Preparação de dados para ferramentas de BI**

---

## 👨‍💻 Autor

**Vinícius Oliveira .-. **

* GitHub: https://github.com/Vinicius0liveira

---

⭐ Projeto desenvolvido para estudo de **Data Analysis com Python** e futura integração com **Power BI e ferramentas de Business Intelligence**.
