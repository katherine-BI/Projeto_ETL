## ☕ Projeto ETL e Visualização de Dados: Desafio de Business Intelligence

---

### 1. Descrição

Este projeto de **ETL (Extract, Transform, Load)** e **Visualização de Dados** foi desenvolvido como parte do desafio de **Business Intelligence (BI)** do bootcamp oferecido pela **WomakersCode** em parceria com o **Instituto Localiza**. A execução e análise foram realizadas pela *Squad Katherine Johnson*.

O projeto tem como base um cenário hipotético: a abertura de uma nova cafeteria. Para garantir a assertividade no *mix* de produtos e serviços, foi realizada uma análise exploratória e preditiva sobre os padrões de consumo de café na região do *dataset* original.

---

### 2. Objetivo

O objetivo principal é transformar dados brutos de consumo de café em informações estratégicas e *insights* acionáveis, utilizando um processo de ETL estruturado e visualizações interativas no **Power BI**.

As análises visam responder às seguintes hipóteses de negócio para direcionar a estratégia da nova cafeteria:

1.  **Bebida favorita por gênero:** Identificar as preferências de bebidas com café entre diferentes gêneros.
2.  **Ambiente de consumo:** Determinar onde o café é mais frequentemente consumido (e.g., em casa, no trabalho, em cafeterias).
3.  **Sabores preferidos no teste:** Entender quais sabores (do *tasting* realizado) obtiveram maior preferência.
4.  **Top 10 sabores mais consumidos:** Listar os 10 sabores de café mais populares ou frequentemente escolhidos.
5.  **Razões para beber café:** Investigar as motivações primárias que levam os consumidores a beber café (e.g., energia, socialização, sabor).

---

### 3. Estrutura do Projeto

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

### 4. Passos de Execução

Segue o fluxo de trabalho detalhado para replicação do projeto:

#### **4.1. Configuração e Extração (Bronze)**

1.  **Download do Dataset:** Obter o arquivo CSV ou o *dataset* completo da fonte Kaggle.
2.  **Criação dos Schemas/Estruturas:** Criar os três *schemas* ou diretórios de armazenamento (`BRONZE`, `SILVER`, `GOLD`).
3.  **Carregamento para Bronze:** Ingerir os dados brutos, **sem modificação**, para a camada `BRONZE`.

#### **4.2. Transformação (Silver)**

1.  **Leitura do Bronze:** Ler os dados da camada `BRONZE`.
2.  **Limpeza e Padronização:**
    * Tratar valores ausentes (NULLs).
    * Corrigir *data types* e formatos inconsistentes.
    * Renomear colunas para maior clareza.
3.  **Escrita no Silver:** Persistir os dados limpos na camada `SILVER`.

#### **4.3. Consolidacão (Gold)**

1.  **Leitura do Silver:** Ler os dados limpos da camada `SILVER`.
2.  **Aplicação das Regras de Negócio:**
    * Criar colunas calculadas relevantes para as hipóteses (ex: categorização de faixa etária).
    * Realizar agregações e sumarizações necessárias (ex: contagem de frequência de sabores).
    * Realizar **junções de tabelas** (se houver) para criar o modelo de dados final.
3.  **Escrita no Gold:** Persistir o modelo de dados final, pronto para consumo, na camada `GOLD`.

#### **4.4. Visualização (Power BI)**

1.  **Conexão com Gold:** Conectar o Power BI à camada `GOLD`.
2.  **Modelagem de Dados:** Criar o modelo de dados (*relationships*) e definir medidas (DAX).
3.  **Desenvolvimento do Dashboard:** Construir gráficos e visuais que enderecem diretamente as 5 hipóteses levantadas.
4.  **Publicação:** Publicar o *report* para compartilhamento.

---

### 5. Resultados e Prints

O *dashboard* final do Power BI contém visualizações interativas que permitem explorar as tendências de consumo e validar as hipóteses de negócio.

> **Nota:** Os prints devem ser inseridos aqui, representando as telas do Power BI que respondem às hipóteses.

* [**Print 1:** Dashboard Principal com KPIs e filtros]
* [**Print 2:** Gráfico de Bebida Favorita por Gênero (Resposta à Hipótese 1)]
* [**Print 3:** Gráfico de Top 10 Sabores Mais Consumidos (Resposta à Hipótese 4)]
