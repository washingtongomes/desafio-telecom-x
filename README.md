#  Data Science - Oracle - OneG9 - Alura
![Python](https://img.shields.io/badge/Python-3.10+-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange)

# DESAFIO TELECOM-X 
# 📊 Análise de Evasão de Clientes (Churn) — TelecomX

---

## 1. Introdução

A evasão de clientes (Churn) é um dos principais desafios enfrentados por empresas de telecomunicações, pois impacta diretamente a receita, os custos de aquisição de novos clientes e a sustentabilidade do negócio.

O objetivo desta análise é **compreender o comportamento dos clientes que cancelaram o serviço**, identificando padrões e fatores associados à evasão. A partir desses insights, busca-se apoiar decisões estratégicas voltadas à **retenção de clientes**, melhoria de serviços e redução do churn.

---

## 2. Limpeza e Tratamento de Dados

Nesta etapa, os dados foram preparados para garantir consistência, qualidade e confiabilidade das análises.

### 🔹 Importação dos dados
- Os dados foram importados a partir de um arquivo JSON disponibilizado via link do GitHub.
- Após o carregamento, os dados foram convertidos em um DataFrame do Pandas para facilitar o processamento.

### 🔹 Tratamento de tipos de dados (dtype)
- Conversão de colunas numéricas que estavam como texto, como:
  - `account.Charges.Total`
- Garantia de tipos corretos:
  - Variáveis numéricas: `int64` e `float64`
  - Variáveis categóricas: `object`

### 🔹 Criação de novas variáveis
- **`contas_diaria`**: criada a partir do faturamento mensal dividido por 30, permitindo uma visão mais granular do custo do cliente.
- Padronização de valores categóricos, facilitando análises estatísticas e visuais.

### 🔹 Tratamento de valores ausentes
- Registros com valores nulos em colunas financeiras foram tratados para evitar distorções nas análises.

---

## 3. Análise Exploratória de Dados (EDA)

A Análise Exploratória teve como foco entender **como o churn se distribui** e **quais fatores estão mais associados à evasão**.

### 📌 3.1 Distribuição do Churn
- Foi analisada a proporção de clientes que:
  - Permaneceram
  - Cancelaram o serviço
- O gráfico de barras horizontal evidenciou que, embora a maioria dos clientes permaneça, uma parcela relevante cancela o serviço, justificando a necessidade de ações preventivas.

---

### 📌 3.2 Churn por Variáveis Categóricas
Foram analisadas variáveis como:
- Gênero
- Tipo de contrato
- Método de pagamento
- Serviços adicionais

**Principais observações:**
- Clientes com **contratos mensais** apresentam maior taxa de evasão.
- Métodos de pagamento automáticos tendem a estar associados a menor churn.
- A ausência de serviços adicionais (como suporte técnico e segurança online) está relacionada a maior propensão ao cancelamento.

---

### 📌 3.3 Churn por Variáveis Numéricas
Foram comparadas as distribuições de clientes que cancelaram e não cancelaram utilizando boxplots.

#### 🔹 Tempo de contrato (tenure)
- Clientes que cancelaram possuem, em média, **menos tempo de permanência**.
- Indica que os primeiros meses são críticos para retenção.

#### 🔹 Total gasto
- Clientes que permanecem tendem a apresentar **maior gasto acumulado**, reflexo do maior tempo de contrato.

#### 🔹 Custo diário
- Clientes com **custo diário mais elevado** demonstram maior sensibilidade ao cancelamento, sugerindo influência do preço na decisão de evasão.

---

## 4. Conclusões e Insights

A análise revelou padrões claros relacionados ao churn:

- ⏳ Clientes com **menor tempo de contrato** são mais propensos a cancelar.
- 💰 **Custos mais altos**, especialmente quando percebidos no curto prazo, aumentam o risco de evasão.
- 📄 **Contratos mensais** apresentam maior churn em comparação a contratos mais longos.
- 🔧 Clientes sem serviços adicionais tendem a cancelar com maior frequência.


---
     

## Equipe

<div align="center">

🔗 **Autor: Washington Gomes**  

<a href="https://github.com/washingtongomes">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" width="100" />
</a>

<br>

🔗 **GitHub:** https://github.com/washingtongomes   
🔗 **Projeto:** https://github.com/washingtongomes/desafio-telecom-x/blob/main/TelecomX_BR.ipynb   
</div>