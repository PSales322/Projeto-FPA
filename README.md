# Painel de Acompanhamento Orçamentário

Painel interativo para acompanhamento do orçamento, análise de desempenho financeiro e projeção de resultados ao longo do exercício.

A aplicação permite comparar valores orçados e realizados, identificar desvios, analisar resultados por unidade e conta e acompanhar o forecast anual a partir dos dados disponíveis.

🔗 **Acesse o painel:** [Painel de Acompanhamento Orçamentário](https://psales322.github.io/Projeto-FPA/)

---

## 🎯 Objetivo do projeto

Desenvolver uma ferramenta visual de apoio ao planejamento e controle orçamentário, facilitando a leitura dos resultados e a identificação de pontos que demandam acompanhamento.

O painel foi estruturado para apoiar análises em diferentes níveis, desde a visão consolidada da cooperativa até o detalhamento por grupo de contas, conta e agência.

---

## 📊 Funcionalidades

### 1. Visão executiva
Apresenta uma visão consolidada do desempenho orçamentário, com indicadores, comparações e destaques para facilitar a leitura dos resultados.

### 2. Análise de receitas
Permite acompanhar o desempenho das receitas em relação ao orçamento, identificar desvios e observar sua evolução ao longo do período.

### 3. Análise de despesas
Apresenta o comportamento das despesas orçadas e realizadas, com análise de desvios e detalhamento por grupos e contas.

### 4. Análise de Agências × Sede
Permite comparar o desempenho das agências com o da sede, identificar a origem dos resultados e detalhar informações por agência.

### 5. Forecast
Apresenta a projeção de fechamento anual, considerando o realizado acumulado e o comportamento esperado para os meses restantes.

O painel disponibiliza métodos de projeção baseados no acumulado do ano e nos últimos 3 ou 6 meses, além de permitir ajustes de parâmetros e cenários.

### 6. Filtros e navegação
A análise pode ser personalizada por meio de filtros de:

- Mês de referência;
- Visão acumulada no ano ou somente do mês;
- Unidade: cooperativa, agências ou sede;
- Agência;
- Natureza: resultado, receitas ou despesas;
- Grupo de contas;
- Conta.

Também é possível limpar os filtros e navegar entre as páginas do painel.

### 7. Detalhamento e análise de desvios
O painel apresenta tabelas e gráficos para comparar orçamento e realizado, identificar desvios em valores e percentuais e explorar informações por conta e agência.

A classificação dos desvios considera a natureza analisada: em receitas, desvios positivos são favoráveis; em despesas, desvios negativos são favoráveis.

### 8. Importação de dados
Permite carregar uma base própria por meio de arquivo CSV, substituindo os dados simulados utilizados na demonstração.

A leitura do arquivo é realizada diretamente no navegador. Os dados importados não são enviados a um servidor pela aplicação.

### 9. Parâmetros de análise
Permite ajustar limites de materialidade para classificação dos desvios em níveis de impacto.

---

## 🧰 Tecnologias utilizadas

- **HTML5:** estrutura e organização do conteúdo;
- **CSS3:** identidade visual, layout responsivo, temas claro e escuro e estilos dos componentes;
- **JavaScript:** filtros, cálculos, processamento dos dados, interações, tabelas e gráficos;
- **SVG:** representação visual dos gráficos;
- **Google Fonts:** tipografia Exo 2 e Nunito;
- **GitHub Pages:** hospedagem e publicação do painel.

O projeto é uma aplicação front-end estática, sem necessidade de servidor próprio ou banco de dados para sua execução.

---

## 🚀 Como utilizar

1. Acesse o [painel publicado](https://psales322.github.io/Projeto-FPA/).
2. Explore as páginas e os filtros disponíveis.
3. Para utilizar uma base própria, clique em **Carregar base**.
4. Selecione um arquivo CSV no formato esperado.
5. Analise os resultados e navegue entre as páginas.

O painel inicia com dados simulados para demonstração. A importação de uma base substitui esses dados durante a utilização.

---

## 📄 Formato da base CSV

O arquivo deve conter uma linha por mês, conta e agência, com as seguintes colunas:

| Campo | Descrição |
|---|---|
| `ano` | Ano de referência |
| `mes` | Mês, de 1 a 12 |
| `natureza` | Receita ou Despesa |
| `grupo` | Grupo da conta |
| `codigo` | Código da conta |
| `conta` | Descrição da conta |
| `origem` | Agência ou Sede |
| `agencia` | Identificação da agência |
| `orcado` | Valor orçado |
| `realizado` | Valor realizado |

### Orientações para o CSV

- Os valores de orçamento e realizado devem ser informados em reais e positivos.
- Para meses futuros, deixe o campo `realizado` em branco.
- O arquivo pode utilizar vírgula ou ponto e vírgula como separador.
- Confira se os nomes das colunas estão de acordo com o formato esperado pelo painel.

---

## 🧮 Lógica do forecast

O forecast considera o realizado acumulado e aplica um fator de performance sobre o orçamento restante.

De forma simplificada:

**Forecast = Realizado acumulado + Orçamento restante × Fator de performance**

O resultado é uma projeção de fechamento anual, não uma garantia do valor que será realizado.

---

## 🔒 Dados e privacidade

A versão publicada utiliza dados simulados para demonstração.

Ao utilizar uma base própria, não publique arquivos que contenham informações confidenciais, dados pessoais ou informações internas sem autorização. A importação do CSV é feita localmente no navegador, mas qualquer arquivo enviado ao repositório público do GitHub poderá ser acessado por outras pessoas.

---

## 📌 Observação

Este projeto tem finalidade demonstrativa e de apoio à análise orçamentária. Os resultados dependem da qualidade, consistência e atualização dos dados utilizados.

---

## 👤 Projeto

Desenvolvido como projeto de análise e acompanhamento orçamentário, com foco em visualização de dados, controle de desempenho e projeção financeira.
