# Challenger2_Telecom-X
Challenger2 do curso de Data Science, análise de evasão de clientes.
# Análise de Evasão de Clientes (Churn) - Telecom X 📊💔

Este projeto tem como objetivo analisar os dados de clientes da Telecom X para identificar os fatores que contribuem para a evasão de clientes (churn) e fornecer insights para estratégias de retenção.

## Dados 📁🔗

Os dados utilizados nesta análise foram obtidos de um arquivo JSON disponível em um repositório GitHub. O dataset contém informações sobre o perfil dos clientes, serviços de telefone e internet, e dados da conta, incluindo se o cliente cancelou o serviço.

## Análise e Processamento de Dados ⚙️🔬

As seguintes etapas foram realizadas para preparar e analisar os dados:

### Carregamento dos Dados
*   Os dados foram carregados diretamente da URL do arquivo JSON para um DataFrame pandas.

### Exploração Inicial
*   Foi realizada uma exploração inicial para entender a estrutura dos dados, verificar tipos de dados, identificar valores nulos e obter estatísticas descritivas.

### Normalização dos Dados
*   As colunas aninhadas (`'customer'`, `'phone'`, `'internet'`, `'account'`) foram normalizadas e combinadas com o DataFrame principal.

### Tratamento de Dados
*   A coluna `Charges.Total` foi convertida para tipo numérico, tratando possíveis erros e preenchendo valores nulos com a mediana.
*   Valores como `'No internet service'` e `'No phone service'` foram padronizados para `'No'` nas colunas de serviços correspondentes.
*   Variáveis binárias foram convertidas para 0 e 1 para facilitar a análise.
*   Nomes de colunas foram padronizados (minúsculas e substituição de espaços por underscores).
*   Duplicatas foram removidas.
*   Valores nulos nas colunas numéricas foram preenchidos com a mediana.

### Análise Exploratória de Dados (EDA)
*   Análise da distribuição geral de churn.
*   Análise da distribuição de churn por gênero, tipo de contrato, encargos mensais e totais, e tempo de contrato (tenure).
*   Cálculo de estatísticas descritivas para variáveis numéricas agrupadas por churn.

## Principais Insights da Análise de Churn ��

A análise exploratória revelou os seguintes fatores chave associados à evasão de clientes:

*   **Tipo de Contrato:** Clientes com contratos mês a mês apresentam uma probabilidade significativamente maior de cancelar o serviço em comparação com aqueles com contratos de longo prazo (um ou dois anos).
*   **Encargos Mensais:** Clientes com encargos mensais mais altos tendem a ter uma maior propensão ao churn.
*   **Tempo de Contrato (Tenure):** Clientes com menor tempo de contrato na empresa são mais propensos a cancelar.
*   **Gênero:** Não foi observada uma diferença significativa na taxa de churn entre homens e mulheres.

## Conclusão ✅🎯

Os insights obtidos sugerem que a Telecom X deve focar suas estratégias de retenção em clientes com contratos mês a mês, aqueles com encargos mensais elevados e clientes com menor tempo de contrato. Ações como oferecer incentivos para contratos de longo prazo e revisar a estrutura de preços para clientes com altos encargos podem ser eficazes.

## Como Executar o Projeto 🐍

Para replicar esta análise, siga os passos abaixo:

1.  **Clone o repositório:**
    ```bash
    git clone https://github.com/seu-usuario/seu-repositorio.git
    cd seu-repositorio
    ```
2.  **Instale as dependências:**
    Certifique-se de ter Python instalado. As principais bibliotecas utilizadas são `pandas` para manipulação de dados e `json` para carregamento (geralmente já incluído no Python padrão).
    ```bash
    pip install pandas
    ```
3.  **Execute o notebook/script:**
    Se o seu projeto inclui um notebook Jupyter (`.ipynb`) ou um script Python (`.py`), você pode executá-lo para reproduzir a análise.

    Exemplo para Jupyter Notebook:
    ```bash
    jupyter notebook
    ```
    Exemplo para script Python:
    ```bash
    python seu_script_de_analise.py
    ```

---
Espero que ajude! 😊
