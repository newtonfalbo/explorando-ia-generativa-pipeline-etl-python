# Explorando IA Generativa em um Pipeline de ETL com Python

## 📖 Descrição

Este projeto demonstra a aplicação prática de um pipeline **ETL (Extract, Transform and Load)** enriquecido com **Inteligência Artificial Generativa**, utilizando Python e o modelo Gemini.

O objetivo é extrair dados de clientes, realizar transformações para classificação de perfil financeiro e gerar recomendações personalizadas por meio de IA, armazenando os resultados em um novo conjunto de dados.

Projeto desenvolvido como desafio prático do bootcamp de Ciência de Dados com Python da DIO.

---

## Objetivos

* Aplicar os conceitos de ETL utilizando Python.
* Realizar tratamento e enriquecimento de dados com Pandas.
* Utilizar IA Generativa para produzir recomendações financeiras personalizadas.
* Demonstrar a integração entre Ciência de Dados e Inteligência Artificial.

---

## Tecnologias Utilizadas

* Python
* Pandas
* Google Gemini API
* Google Colab
* Jupyter Notebook
* GitHub

---

## Pipeline ETL

### 1 Extract

Nesta etapa, os dados dos clientes são carregados para o ambiente de análise.

Exemplo dos dados utilizados:

| ID | Nome   | Idade | Renda |
| -- | ------ | ----- | ----- |
| 1  | Ana    | 25    | 3500  |
| 2  | Carlos | 42    | 8000  |
| 3  | Marina | 31    | 5500  |
| 4  | Pedro  | 58    | 12000 |
| 5  | Lucas  | 22    | 2500  |

---

### 2 Transform

Os dados passam por transformações e enriquecimento.

Foi criada uma classificação de faixa de renda:

* Baixa
* Média
* Alta

Essa classificação é utilizada posteriormente pela IA para personalizar as recomendações.

---

### 3 IA Generativa

Utilizando o modelo Gemini, o projeto gera recomendações financeiras personalizadas para cada cliente com base em:

* Nome
* Idade
* Renda
* Faixa de renda

Exemplo:

> "Priorize a construção de uma reserva de emergência antes de investir."

---

### 4 Load

Os dados enriquecidos são armazenados em um novo arquivo CSV contendo as recomendações geradas.

Exemplo de saída:

| Nome   | Faixa de Renda | Insight IA                             |
| ------ | -------------- | -------------------------------------- |
| Ana    | Baixa          | Priorize uma reserva de emergência.    |
| Carlos | Média          | Diversifique seus investimentos.       |
| Pedro  | Alta           | Proteja e diversifique seu patrimônio. |

---

## Resultados

O pipeline ETL foi executado com sucesso, demonstrando como a Inteligência Artificial Generativa pode agregar valor aos dados por meio da criação de insights personalizados.

---

## Estrutura do Projeto

```text
 projeto-etl-ia-generativa
 ┣  ETL_IA_Generativa.ipynb
 ┣  clientes_com_insights.csv
 ┗  README.md
```

---

## Como Executar

1. Clone este repositório:

```bash
git clone <url-do-repositorio>
```

2.Abra o notebook no Google Colab ou Jupyter Notebook.

3.Instale as dependências:

```bash
pip install pandas google-generativeai
```

4.Configure sua chave da API Gemini.

5.Execute todas as células do notebook.

---

## Autor

Newton Falbo

Projeto desenvolvido durante o bootcamp de Ciência de Dados com Python da DIO, explorando conceitos de ETL e Inteligência Artificial Generativa aplicados ao contexto financeiro.
