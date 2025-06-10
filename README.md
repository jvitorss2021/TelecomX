# Análise de Evasão de Clientes (Churn) em Empresa de Telecomunicações

![Status do Projeto](https://img.shields.io/badge/status-concluído-green)
![Linguagem](https://img.shields.io/badge/python-3.x-blue)
![Bibliotecas](https://img.shields.io/badge/pandas-matplotlib-seaborn)

---

## 📄 Descrição do Projeto

> Este projeto realiza uma análise exploratória completa sobre um conjunto de dados de uma empresa de telecomunicações. O objetivo principal é identificar os principais fatores e perfis de clientes que levam à evasão (Churn), fornecendo insights valiosos que possam direcionar estratégias de negócio para aumentar a retenção de clientes.

---

## 🚀 Estrutura da Análise

O projeto foi estruturado em um notebook Jupyter (`.ipynb`) seguindo as seguintes etapas:

1.  **Extração e Limpeza de Dados:**
    * Importação dos dados a partir de um arquivo JSON.
    * Tratamento de uma estrutura de dados aninhada utilizando `pandas.json_normalize` para criar um DataFrame funcional.
    * Padronização e tradução dos nomes das colunas.
    * Conversão de dados categóricos (ex: 'Yes'/'No') para formato numérico (1/0).
    * Correção de tipos de dados, com destaque para a coluna de Fatura Total.

2.  **Análise Exploratória de Dados (EDA):**
    * Análise da taxa de Churn geral para estabelecer uma linha de base.
    * Visualização da relação entre **variáveis categóricas** (Tipo de Contrato, Método de Pagamento, etc.) e o Churn, utilizando gráficos de barras.
    * Análise da distribuição de **variáveis numéricas** (Meses de Contrato, Fatura Mensal) entre os grupos de clientes (Churn vs. Não Churn), utilizando gráficos de violino para uma visualização detalhada da densidade.

3.  **Relatório Final:**
    * Consolidação de todos os insights em um relatório estruturado, detalhando o processo e as conclusões.

---

## 📊 Principais Insights Gerados

A análise revelou perfis de clientes e características de serviços que estão fortemente correlacionados com a evasão:

* **Tipo de Contrato:** É o fator de maior impacto. Clientes com contrato **mensal (Month-to-month)** possuem uma taxa de churn drasticamente superior.
* **Fatura Mensal:** Existe uma "zona de perigo" de faturamento entre **R$ 70 e R$ 105**, onde a concentração de clientes que cancelam é máxima.
* **Tempo de Contrato (Tenure):** A evasão é um fenômeno que ocorre majoritariamente no **início do ciclo de vida do cliente**, com a maioria dos cancelamentos acontecendo nos primeiros meses.
* **Método de Pagamento:** O pagamento via **Boleto Eletrônico (Electronic Check)** está associado a uma taxa de churn muito mais alta em comparação com métodos automáticos (Cartão de Crédito e Débito em Conta).

---

## 💡 Recomendações Estratégicas

Com base nos insights, foram propostas as seguintes ações para a área de negócio:

1.  **Incentivar Contratos de Longo Prazo:** Criar campanhas ativas para migrar clientes do plano mensal para contratos anuais, oferecendo benefícios claros.
2.  **Monitorar a "Zona de Perigo":** Implementar ações de retenção proativas para clientes cuja fatura mensal se encontra na faixa de R$ 70-R$105.
3.  **Fortalecer o Onboarding:** Desenvolver um programa de engajamento para clientes nos primeiros meses para garantir uma percepção de valor positiva desde o início.
4.  **Reduzir Atrito no Pagamento:** Incentivar a migração de clientes do boleto para métodos de pagamento automático.

---

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** `Python 3`
* **Bibliotecas:**
    * `Pandas` para manipulação e análise de dados.
    * `Matplotlib` e `Seaborn` para visualização de dados.
* **Ambiente:** `Google Colab`

---

## ⚙️ Como Executar o Projeto

1.  Clone este repositório:
    ```bash
    git clone https://github.com/jvitorss2021/TelecomX.git
    ```
2.  Abra o arquivo `.ipynb` no Google Colab, Jupyter Notebook ou ambiente compatível.
3.  Execute as células de código em ordem sequencial.

---

## 👨‍💻 Autor

* **João Vitor Sant'Ana**
* **LinkedIn:** [https://www.linkedin.com/in/jo%C3%A3o-vitor-soares-santana/](https://www.linkedin.com/in/jo%C3%A3o-vitor-soares-santana/)

---

## 📜 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
