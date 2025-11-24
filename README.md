<p align="center">
  <img src="https://raw.githubusercontent.com/caiocamposdev/assets/main/banners/data-etl-coffee-banner.png" alt="ETL Coffee Project Banner" width="100%">
</p>

<h1 align="center">☕ Projeto de ETL & BI — Nova Cafeteria</h1>
<h3 align="center">Bootcamp WomakersCode x Instituto Localiza · Squad Katherine Johnson</h3>

<br>

<!-- =============================== -->
<!-- ========== BADGES ============= -->
<!-- =============================== -->

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10+-blue?logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/Google_Colab-Notebook-orange?logo=googlecolab&logoColor=white">
  <img src="https://img.shields.io/badge/Power_BI-Dashboard-F2C811?logo=powerbi&logoColor=black">
  <img src="https://img.shields.io/badge/Kaggle-Dataset-20BEFF?logo=kaggle&logoColor=white">
  <img src="https://img.shields.io/badge/ETL-Data%20Pipeline-green">
  <img src="https://img.shields.io/badge/Status-Concluído-success">
</p>

<br>

---

# 📚 **Sumário**
- [1. Descrição](#-1-descrição)
- [2. Objetivo](#-2-objetivo)
- [3. Arquitetura do Projeto](#-3-arquitetura-do-projeto)
- [4. Passos de Execução](#-4-passos-de-execução)
  - [4.0 Como clonar o repositório](#-40--como-clonar-o-repositório)
  - [4.0.1 Como abrir o notebook no Google Colab](#-401--como-abrir-o-notebook-no-google-colab)
  - [4.0.2 Como abrir o relatório no Power BI](#-402--como-abrir-o-relatório-no-power-bi)
  - [4.1 Extração (BRONZE)](#-41--extração-bronze)
  - [4.2 Transformação (SILVER)](#-42--transformação-silver)
  - [4.3 Consolidação (GOLD)](#-43--consolidação-gold)
  - [4.4 Visualização no Power BI](#-44--visualização-power-bi)
- [5. Resultados](#-5-resultados)
- [6. Autores](#-6-autores)

---

# ✔️ **1. Descrição**

Este projeto de **ETL (Extract, Transform, Load)** e **Visualização de Dados** foi desenvolvido como parte do desafio de **Business Intelligence (BI)** do bootcamp oferecido pela **WomakersCode** em parceria com o **Instituto Localiza**. A execução e análise foram realizadas pela *Squad Katherine Johnson*.

O projeto tem como base um cenário hipotético: a abertura de uma nova cafeteria. Para garantir a assertividade no *mix* de produtos e serviços, foi realizada uma análise exploratória e preditiva sobre os padrões de consumo de café na região do *dataset* original.

---

# 🎯 **2. Objetivo**

Transformar dados brutos em **informações estratégicas**, aplicando:

- ETL com Python (Colab)
- Arquitetura Lakehouse (Bronze → Silver → Gold)
- Dashboards interativos no Power BI
- Insights para apoiar decisões de negócio

As análises visam responder às seguintes hipóteses de negócio para direcionar a estratégia da nova cafeteria:

1.  **Bebida favorita por gênero:** Identificar as preferências de bebidas com café entre diferentes gêneros.
2.  **Ambiente de consumo:** Determinar onde o café é mais frequentemente consumido (e.g., em casa, no trabalho, em cafeterias).
3.  **Sabores preferidos no teste:** Entender quais sabores (do *tasting* realizado) obtiveram maior preferência.
4.  **Top 10 sabores mais consumidos:** Listar os 10 sabores de café mais populares ou frequentemente escolhidos.
5.  **Razões para beber café:** Investigar as motivações primárias que levam os consumidores a beber café (e.g., energia, socialização, sabor).

---

### 🏛️ 3. Estrutura do Projeto

O projeto adota uma arquitetura de *Data Lakehouse* com três camadas distintas (*Bronze, Silver, Gold*), garantindo a rastreabilidade, qualidade e organização dos dados.



| Camada | Descrição | Propósito |
| :--- | :--- | :--- |
| **BRONZE** | Dados **Brutos** (RAW) | Armazena os dados originais (copiados diretamente da fonte) sem qualquer alteração. É a zona de *stage* inicial. |
| **SILVER** | Dados **Transformados** (CLEANSED) | Contém os dados após a aplicação das **principais transformações** e limpezas (tratamento de valores nulos, *outliers*, padronização de formatos, etc.). É a visão de dados prontos para análise inicial. |
| **GOLD** | Dados **Consolidados** (CONSUMPTION) | Contém os dados após aplicação das **regras de negócio**, **agregações** e **junções de tabelas** necessárias para a camada de visualização. É a camada otimizada para consultas de BI e *Dashboards*. |

* **Fonte de Dados:** [Kaggle Dataset: Let's do some coffee tasting](https://www.kaggle.com/datasets/sujaykapadnis/lets-do-some-coffee-tasting/data)
* **Processo de ETL:** Implementado utilizando a linguagem de programação Python (ou ferramentas de ETL).
* **Visualização:** **Power BI** para criação de *dashboards* interativos e *reports* de BI.

---

# 🚀 4. Passos de Execução

---

## 🔹 4.0 — Como clonar o repositório

### **Via HTTPS**
```bash
git clone https://github.com/SEU-USUARIO/NOME-DO-REPOSITORIO.git
```
### **Via SSH**
```git clone git@github.com:[katherine-BI/Projeto_ETL]```

###Depois, entre no diretório:
``` cd "Projeto_ETL" ```

## 🔹 4.0.1 — Como abrir o notebook no Google Colab

### **Opção 1 — Abrir direto pelo botão “Open in Colab”**
- Acesse o arquivo `.ipynb` no GitHub  
- Clique no botão **Open in Colab**

---

### **Opção 2 — Abrir pelo site do Colab**
- Acesse: https://colab.research.google.com  
- Vá em **File → Open Notebook**  
- Clique na aba **GitHub**  
- Pesquise o nome do repositório  
- Selecione o arquivo `.ipynb`

---

### **Opção 3 — Upload manual**
- Baixe o arquivo `.ipynb`  
- No Colab: **File → Upload**  
- Selecione o notebook  

---

## 🔹 4.0.2 — Como abrir o relatório no Power BI

### **Arquivo local (.pbix)**
- Instale o **Power BI Desktop**:  
  https://www.microsoft.com/pt-br/download/details.aspx?id=58494  
- Clique duas vezes no arquivo `.pbix` dentro do repositório  
- O relatório será carregado automaticamente  

---

### **Arquivo na nuvem**
- Faça o download do arquivo `.pbix`  
- Abra no **Power BI Desktop** normalmente  

---

## 🔸 4.1 — Extração (BRONZE)
- Baixar dataset do Kaggle  
- Criar diretórios: `BRONZE`, `SILVER`, `GOLD`  
- Armazenar o dataset original na camada **BRONZE**  

---

## 🔸 4.2 — Transformação (SILVER)

- Ler dados da camada **BRONZE**  
- Aplicar transformações:
  - Tratamento de nulos  
  - Ajuste de tipos  
  - Padronização  
  - Renomeação de colunas  
- Persistir dados transformados na camada **SILVER**

---

## 🔸 4.3 — Consolidação (GOLD)

- Ler dados da camada **SILVER**  
- Criar regras de negócio:
  - Cálculos  
  - Agregações  
  - Junções  
  - Métricas  
- Salvar o modelo final na camada **GOLD**  

---

## 🔸 4.4 — Visualização (Power BI)

- Conectar o Power BI à camada **GOLD**  
- Criar o modelo relacional e medidas DAX  
- Construir o dashboard respondendo às 5 hipóteses  
- Publicar no Power BI Service (opcional)  

---

## 🖼️ 5. Resultados e Prints

O dashboard final apresenta visualizações interativas que permitem explorar tendências de consumo de café, validar hipóteses e identificar oportunidades estratégicas para a nova cafeteria.

---

### Autor
Squad Katherine Johnson - Bootcamp BI WomakersCode 
