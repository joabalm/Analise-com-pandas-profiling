
# 📊 Análise Exploratória com ydata-profiling (antigo pandas-profiling)

Este projeto demonstra como utilizar a biblioteca [ydata-profiling](https://github.com/ydataai/ydata-profiling), anteriormente conhecida como `pandas-profiling`, para gerar relatórios de análise exploratória automática de dados com Python. O notebook foi desenvolvido no [Google Colab](https://colab.research.google.com) utilizando a linguagem `Python` com o suporte das bibliotecas `pandas` e `ydata-profiling`.

---

## 🔗 Links úteis

- 📦 PyPI: [pandas-profiling / ydata-profiling](https://pypi.org/project/pandas-profiling/)
- 💻 Repositório oficial: [github.com/ydataai/ydata-profiling](https://github.com/ydataai/ydata-profiling)
- 📓 Acesse o notebook: [`pandas-profiling.ipynb`](./pandas-profiling.ipynb)

---

## ⚙️ Instalação

Para usar a biblioteca no ambiente do Google Colab ou localmente, execute:

```python
!pip install ydata-profiling
```

---

## 📁 Dependências

- `pandas`
- `ydata-profiling` (versão moderna do `pandas-profiling`)

---

## 🚀 Exemplo de Uso

```python
import pandas as pd
from ydata_profiling import ProfileReport

# Carregando dataset
df = pd.read_csv('nome_do_arquivo.csv')

# Gerando o relatório de perfil
profile = ProfileReport(df, title="Relatório de Análise Exploratória", explorative=True)

# Exibindo no notebook
profile.to_notebook_iframe()

# Salvando como HTML
profile.to_file("relatorio_analise.html")
```

---

## 📈 Resultado

O relatório gerado inclui:

- Estatísticas descritivas completas
- Análise de distribuição de variáveis
- Detecção de colunas com valores ausentes
- Correlações entre variáveis
- Sugestões de limpeza de dados
- Dicionário de variáveis e tipos

---

## 🧪 Ambiente Utilizado

- Google Colab
- Python 3.x
- pandas
- ydata-profiling

---

## 📌 Observações

- A biblioteca `ydata-profiling` é poderosa para gerar análises automatizadas, mas pode consumir bastante memória para datasets muito grandes.
- Para uma análise mais interativa, use a opção `explorative=True`.

---

## 🧑‍💻 Autor

Joab Almeida
