##  Grupo

| Nome            | RM        |
|-----------------|-----------|
| *Thiago nakano* | RM 569151 |
| *Leticia okano* | RM 571988 |
| *Guilherme*  | RM 569658 |

--------------

## Objetivo 

Este projeto tem como objetivo utilizar dados públicos de energia renovável e técnicas de Machine Learning para analisar dois problemas diferentes.

O projeto foi dividido em duas tarefas:

Tarefa 1 — Classificação: utilizar dados de empreendimentos da ANEEL para tentar classificar a fonte de geração como Solar, Eólica ou Hidráulica, usando como entradas a potência e a localização do empreendimento.
Tarefa 2 — Regressão: utilizar dados de radiação solar para construir modelos capazes de estimar a radiação solar em Petrolina (PE).

Em cada tarefa foram utilizados e comparados três algoritmos diferentes, buscando avaliar qual modelo apresenta o melhor desempenho para cada problema.

-------------
## Origem dos dados e Período de dados

**Tarefa 1 — ANEEL**

Os dados da primeira tarefa foram obtidos do conjunto SIGA — Sistema de Informações de Geração da ANEEL.

A consulta utiliza a API pública CKAN/DataStore da ANEEL e considera empreendimentos dos seguintes tipos:

UFV → Solar
EOL → Eólica
UHE → Hidráulica
PCH → Hidráulica
CGH → Hidráulica

Para o modelo, foram utilizadas três entradas:

potencia_kw — potência outorgada do empreendimento em kW;
latitude — latitude aproximada;
longitude — longitude aproximada.

Os registros correspondem aos empreendimentos retornados pela API da ANEEL para as categorias UFV, EOL, UHE, PCH e CGH.

**Tarefa 2 — Radiação Solar**

A segunda tarefa utiliza dados de radiação solar para a cidade de Petrolina, Pernambuco.

O objetivo é utilizar as variáveis disponíveis nos dados para treinar modelos de regressão capazes de estimar a radiação solar

Foram utilizados os dados do período disponibilizado pela API utilizada para a consulta da radiação solar em Petrolina.

---------------

## Período de dados

Na tarefa 1, os dados utilizados no projeto foram obtidos por meio de APIs públicas, sem necessidade de login, token ou chave de API.

Na Tarefa 2, foram utilizados os dados do período disponibilizado pela API utilizada para a consulta da radiação solar em Petrolina.

----------------

## Como executar o projeto

1. Fazer o download do arquivo Aula_APIs_Energia_Renovavel_ML.ipynb no Google Colab
2. Clique no botao Conectar que se encontra no canto superior da tela
3. Depois execute todos os códigos na ordem do notebook

-------------

## Conclusao das Tarefas

Com as duas ultimas aulas, foi possivel aprender mais e por em prática os conceitos de Machine Learning em dois problemas relacionados à energia renovável.

Na primeira tarefa, foi realizado um problema de classificação, no qual os modelos tentaram identificar se um empreendimento era Solar, Eólico ou Hidráulico a partir de sua potência e localização.

Na segunda tarefa, foi realizado um problema de regressão, utilizando dados de radiação solar de Petrolina para estimar um valor numérico.

A comparação entre diferentes algoritmos permitiu observar que cada modelo possui características e desempenhos diferentes dependendo do problema e dos dados utilizados.

De forma geral, o projeto mostrou como dados obtidos de APIs públicas podem ser organizados e utilizados para criar modelos de Machine Learning, além de demonstrar a importância de comparar diferentes algoritmos e métricas antes de escolher um modelo.
