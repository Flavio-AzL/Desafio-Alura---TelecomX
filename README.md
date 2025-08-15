# Análise de Evasão de Clientes (Churn) - Desafio Telecom X

## 📄 Descrição do Projeto
Este projeto consiste em uma análise exploratória de dados (EDA) sobre a evasão de clientes (churn) em uma empresa fictícia de telecomunicações, a Telecom X. O objetivo principal é identificar os fatores que mais contribuem para o cancelamento de serviços por parte dos clientes, a fim de fornecer insights valiosos que possam orientar a criação de estratégias de retenção mais eficazes.

Este repositório contém o notebook com todo o processo de análise, desde a coleta e limpeza dos dados até a geração de visualizações e a consolidação dos insights em um relatório final.

## 🎯 Contexto do Desafio
Este trabalho foi desenvolvido como parte do Desafio "Telecom X - Análise de Evasão de Clientes". O projeto visa aplicar na prática os conhecimentos em Python e suas principais bibliotecas de análise de dados para resolver um problema de negócio real.

## 🛠️ Ferramentas e Bibliotecas Utilizadas
* **Linguagem:** Python
* **Ambiente:** Google Colab
* **Bibliotecas:**
  * **Pandas:** Para manipulação, limpeza e transformação dos dados (ETL).
  * **Numpy:** Para operações numéricas.
  * **Matplotlib & Seaborn:** Para a criação de visualizações de dados.
* **Controle de Versão:** Git e GitHub

## 📁 Estrutura do Repositório
O projeto está organizado da seguinte forma:
```
/
├── dados/
│   └── TelecomX_Data.json      # Dados brutos fornecidos para o desafio
├── notebooks/
│   └── Analise_Churn_TelecomX.ipynb # Notebook contendo toda a análise
└── README.md                   # Este arquivo explicativo
```

## 🚀 Como Executar o Projeto
1.  Clone este repositório para a sua máquina local.
2.  Abra o Google Colab ([colab.research.google.com](https://colab.research.google.com)).
3.  Faça o upload do notebook `Analise_Churn_TelecomX.ipynb` que está na pasta `/notebooks`.
4.  Quando o notebook solicitar, faça o upload do arquivo de dados `TelecomX_Data.json`.
5.  Execute as células do notebook em sequência para reproduzir a análise.

## 📈 Resumo das Etapas do Projeto
O projeto foi desenvolvido seguindo as principais etapas de um processo de análise de dados:

1.  **Extração dos Dados:** Carregamento do arquivo JSON para um DataFrame do Pandas.
2.  **Transformação e Limpeza (ETL):**
    * Desempacotamento de colunas aninhadas (`customer`, `phone`, `internet`, `account`).
    * Correção de tipos de dados (ex: `Charges.Total` de texto para numérico).
    * Tratamento de valores inconsistentes (ex: strings vazias na coluna `Churn`).
    * Engenharia de Atributos (criação da coluna `Contas_Diarias`).
3.  **Análise Exploratória de Dados (EDA):**
    * Análise da taxa geral de churn.
    * Investigação da relação entre o churn e variáveis-chave como `tenure`, `Contract`, `Charges.Monthly`, `InternetService` e a contratação de serviços adicionais.
4.  **Geração de Relatório:** Consolidação dos insights em um relatório final com recomendações estratégicas.

## 💡 Principais Insights Gerados
A análise revelou um perfil claro para o cliente com alta propensão ao cancelamento:

* **Contrato Mês a Mês:** Clientes com este tipo de contrato têm uma taxa de churn de **42.7%**, sendo o principal fator de risco.
* **Clientes Novos:** A maioria dos cancelamentos ocorre nos primeiros meses de contrato, indicando falhas na retenção inicial.
* **Serviço de Fibra Ótica:** Apresenta uma taxa de churn (aprox. 42%) mais que o dobro em comparação com o serviço DSL.
* **Faturas Mensais Altas:** Clientes que cancelam tendem a ter um custo mensal mais elevado.
* **Ausência de Serviços Adicionais:** Não contratar serviços como Suporte Técnico ou Segurança Online é um forte indicador de propensão ao churn.

## 👨‍💻 Autor
**FLÁVIO VIEIRA DE ARAÚJO**

* **[LinkedIn](www.linkedin.com/in/flaviovsp)**
* **[GitHub](https://github.com/Flavio-AzL)**
