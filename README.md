# 📊 Análise de Dados de Telefonia Móvel no Brasil

Este projeto realiza uma análise dos dados de telefonia móvel no Brasil, explorando padrões de acesso por **tecnologia, sinal, região** e **tempo**. Utilizamos visualizações dinâmicas e estáticas para identificar tendências e outliers nos acessos de cada estado e região, de 2009 a 2021. 🌐📶

## ⚙️ Funcionalidades

- Visualização dos padrões de acesso por tecnologia e sinal 📶
- Análise temporal e regional de acessos por estado e região 🗺️📈
- Detecção de outliers e tendências regionais
- Gráficos interativos e estáticos para uma experiência visual completa:
  - Barras e pizza 🍕
  - Mapas de calor e bolhas 🔥
  - Gráficos de linha e boxplot 📉

## 🛠️ Tecnologias Utilizadas

- **Pandas**: Manipulação e agregação de dados
- **Geopandas**: Análise espacial para mapas
- **Matplotlib e Seaborn**: Gráficos estáticos e análise de outliers
- **Plotly**: Gráficos interativos para visualização dinâmica

## 🗂️ Estrutura do Projeto

- **`acessos_dados/br_anatel_telefonia_movel_ddd.csv`**: Arquivo com os dados de acessos móveis
- **`gr/`**: Pasta que contém os arquivos do **mapa das Grandes Regiões do Brasil** em formato shapefile, essenciais para a visualização geoespacial no projeto:
  - **`grandes_regioes_shp.shp`**: Arquivo principal com as informações geográficas.
  - **`grandes_regioes_shp.dbf`**: Banco de dados associado que contém os atributos (ex: nomes e siglas das regiões).
  - **`grandes_regioes_shp.shx`**: Índice que facilita a leitura das formas geométricas.
  - **`grandes_regioes_shp.prj`**: Define o sistema de coordenadas (SIRGAS 2000) 🌍.
  - **`grandes_regioes_shp.txt`**: Metadados do shapefile, descrevendo a fonte dos dados (IBGE) e informações detalhadas sobre o arquivo.
  - **`grandes_regioes_shp.jpg`**: Imagem de visualização do mapa.
- **`main.ipynb`**: Notebook Jupyter que contém o código principal para a análise e visualização dos dados 📊.
- **`requirements.txt`**: Arquivo contendo as dependências do projeto, necessárias para instalar as bibliotecas usadas.
- **`.gitignore`**: Arquivo de configuração para ignorar arquivos desnecessários no Git.
- **`README.md`**: Documentação e instruções do projeto

## 🚀 Como Rodar

### Pré-requisitos

- **Python 3.8+** 
- Bibliotecas necessárias (instalação abaixo) 🛠️

### Instalação

1. Clone o repositório:
   ```
   git clone https://github.com/NicolasVitorCarvalhodeOliveira/data-analysis-mobile-access-br.git
   cd data-analysis-mobile-access-br
   ```

2. Instale as dependências:
   ```
   pip install -r requirements.txt
   ```

3. Certifique-se de que o arquivo `br_anatel_telefonia_movel_ddd.csv` está no diretório `acessos_dados/`.

### ⌨️ Execução

- **Modo Notebook**: Para executar a análise e gerar as visualizações 📊, abra o arquivo `main.ipynb` no Jupyter Notebook:
  ```
  jupyter notebook main.ipynb
  ```
