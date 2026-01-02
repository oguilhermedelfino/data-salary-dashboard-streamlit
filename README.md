<p align="center">
  📊
</p>

<h1 align="center">
  Data Salary Dashboard
</h1>

<p align="center">
  Painel interativo de Business Intelligence desenvolvido em <strong>Python</strong> e <strong>Streamlit</strong> para análise exploratória de dados salariais globais na área de tecnologia.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/python-3.x-blue.svg" alt="Python">
  <img src="https://img.shields.io/badge/streamlit-framework-ff4b4b.svg" alt="Streamlit">
  <img src="https://img.shields.io/badge/pandas-data-150458.svg" alt="Pandas">
  <img src="https://img.shields.io/badge/plotly-viz-3f4f75.svg" alt="Plotly">
</p>

---

## 🎯 Sobre o Projeto

Este projeto é um **Dashboard de Análise de Dados** focado em carreiras de tecnologia (Data Science, Data Engineering, ML, etc.).

O objetivo é fornecer uma visão clara e interativa sobre como a **senioridade, localização geográfica e tipo de contrato** influenciam a remuneração em Dólar (USD) ao redor do mundo.

O projeto foi desenvolvido durante a **Imersão de Análise de Dados da Alura**, aplicando técnicas de ETL com Pandas e visualização de dados com Plotly.

---

## 🚀 Tecnologias Utilizadas

- <strong>Streamlit</strong><br>
  Framework utilizado para construção da interface web interativa e deploy rápido da aplicação de dados.

- <strong>Pandas</strong><br>
  Responsável pela ingestão, limpeza e manipulação do dataset (`dados-imersao-final.csv`).

- <strong>Plotly Express</strong><br>
  Biblioteca de plotagem gráfica utilizada para criar visualizações dinâmicas, responsivas e mapas geográficos.

- <strong>Python</strong><br>
  Linguagem base para toda a lógica de filtragem e cálculo de métricas.

---

## 📊 Funcionalidades e KPIs

O dashboard oferece uma visão macro e micro dos dados através de:

- 🎛️ <strong>Filtros Dinâmicos (Sidebar)</strong><br>
  Permite segmentar a análise por <strong>Ano, Senioridade, Tipo de Contrato e Tamanho da Empresa</strong>.

- 📈 <strong>Métricas Gerais (KPIs)</strong><br>
  Cards com indicadores chave:
  - Salário Médio Anual (USD)
  - Salário Máximo Registrado
  - Total de Registros na Base
  - Cargo mais frequente

- 🗺️ <strong>Visualizações Gráficas</strong><br>
  - <strong>Ranking de Cargos:</strong> Top 10 cargos com maiores médias salariais.
  - <strong>Distribuição Salarial:</strong> Histograma para identificar faixas de remuneração mais comuns.
  - <strong>Modalidade de Trabalho:</strong> Gráfico de rosca comparando trabalho Remoto, Presencial e Híbrido.
  - <strong>Mapa Global:</strong> Mapa de calor (Choropleth) mostrando a média salarial de Cientistas de Dados por país.

---

## 🛠️ Como Executar o Projeto

### 1️⃣ Pré-requisitos

- Python <strong>3.x</strong> instalado
- Gerenciador de pacotes `pip`

---

### 2️⃣ Instalação das dependências

No terminal, na raiz do projeto, execute:

```bash
pip install -r requirements.txt
```

---

## 3️⃣ Executar o Dashboard

Para iniciar a aplicação localmente, utilize o comando do Streamlit:

```bash
streamlit run app.py
```

O navegador abrirá automaticamente no endereço: <strong>http://localhost:8501</strong>

---

## 🗂️ Estrutura de Dados

O dataset utilizado (dados-imersao-final.csv) está estruturado no formato CSV. Abaixo, o dicionário de dados representando as colunas e seus tipos:

 ```json
 {
  "dataset_schema": [
    {
      "coluna": "ano",
      "tipo": "int",
      "descricao": "Ano de referência do pagamento do salário (Ex: 2023, 2024)"
    },
    {
      "coluna": "senioridade",
      "tipo": "string",
      "valores": ["Junior", "Pleno", "Senior", "Executivo"],
      "descricao": "Nível de experiência do profissional"
    },
    {
      "coluna": "cargo",
      "tipo": "string",
      "descricao": "Título da função (Ex: Data Scientist, ML Engineer)"
    },
    {
      "coluna": "usd",
      "tipo": "float",
      "descricao": "Salário anual bruto convertido para Dólar Americano"
    },
    {
      "coluna": "residencia_iso3",
      "tipo": "string",
      "descricao": "Código ISO de 3 letras do país de residência (Ex: BRA, USA)"
    },
    {
      "coluna": "remoto",
      "tipo": "int",
      "valores": [0, 50, 100],
      "descricao": "Percentual de trabalho remoto (0=Presencial, 100=Remoto)"
    },
    {
      "coluna": "tamanho_empresa",
      "tipo": "string",
      "descricao": "Classificação do porte da empresa contratante"
    }
  ]
}
```

---

## 🌐 Deploy

O projeto está disponível online através do Streamlit Cloud:

🔗 <strong>Acessar Dashboard:</strong>

<em></em>

---

## 👤 Autor

Desenvolvido por <strong>Guilherme Delfino</strong>