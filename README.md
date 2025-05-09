# 📊 Segmentação de Clientes com K-Means
## Identificando Perfis de Clientes para Estratégias de Marketing Direcionadas

Este projeto aplica técnicas de machine learning não supervisionadas para segmentar clientes de um shopping center com base em suas características demográficas e comportamentais. O objetivo é identificar grupos com perfis semelhantes, auxiliando em estratégias de marketing direcionadas e personalizadas.

## 🧠 Técnicas Utilizadas
* Label Encoding para variáveis categóricas
* StandardScaler para normalização dos dados
* Análise de Correlação para avaliar a relação linear entre variáveis
* Método do Cotovelo para determinar o número ideal de clusters
* K-Means Clustering para segmentação
* Análise de distribuição por cluster

## 📁 Estrutura dos Dados
As principais colunas utilizadas no projeto são:

* `idade`: idade do cliente
* `renda_anual_k`: renda anual em milhares de dólares
* `pontuacao_gastos`: pontuação de 1 a 100 atribuída pelo shopping com base no histórico de compras e comportamento do cliente
* `genero`: gênero do cliente (Male / Female)
* `genero_encoded`: versão numérica codificada da coluna `genero`
* `Cluster`: o cluster ao qual cada cliente foi atribuído pelo modelo K-Means

## 📈 Resultados
A análise da matriz de correlação revelou uma baixa correlação linear entre as variáveis principais, o que sugere que o K-Means pode ser eficaz para identificar agrupamentos baseados em distância euclidiana. O método do cotovelo indicou que 6 clusters é um número adequado para a segmentação dos clientes. Cada cliente foi atribuído a um cluster específico, facilitando a análise das características de cada grupo. A visualização dos clusters (Renda Anual vs. Pontuação de Gasto) permitiu observar a formação de segmentos distintos.

### Exemplos de Insights:

O Cluster 4 agrupa clientes jovens com baixo poder aquisitivo, mas com uma alta pontuação de gastos.
Outros clusters reúnem pessoas mais velhas com uma renda anual maior e um comportamento de consumo mais moderado (por exemplo, Cluster 0).
A análise da distribuição de gênero dentro de cada cluster revelou padrões de segmentação que podem ser úteis para campanhas de marketing direcionadas a grupos específicos.
## 📊 Próximos Passos 
Explorar outros algoritmos de clustering (por exemplo, DBSCAN, Agglomerative Clustering).
Incorporar mais variáveis ao modelo, se dados adicionais estiverem disponíveis.
Realizar uma análise de perfil mais aprofundada das características de cada cluster.
Integrar os resultados com ferramentas de visualização de dados como o Power BI para criar dashboards interativos e monitorar os segmentos de clientes.
