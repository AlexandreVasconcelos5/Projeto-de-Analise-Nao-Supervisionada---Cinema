## Projeto de Data Science e Análise Não-Supervisionada - Cinema 🎬
Este projeto aplica um ciclo end-to-end de Ciência de Dados com Análise Não-Supervisionada, explorando padrões ocultos e a deteção de valores atípicos em sessões de cinema. O conjunto de dados contém variáveis relacionadas com o preço dos bilhetes, a capacidade das salas, os horários e a ocupação, tendo como variável-alvo Receita_Total. O foco principal do projeto foi segmentar sessões de cinema em perfis distintos através de clustering e detetar anomalias relevantes, permitindo compreender fenómenos como preços fora do normal, ocupações invulgares ou sessões premium.
________________________________________

## Destaques do Projeto
- Projeto avaliado com 18 valores, refletindo rigor e profundidade na aplicação de técnicas de data science e análise não-supervisionada.
- Conjunto de dados real com 142.524 registos e 14 variáveis.
- Tratamento dos valores omissos através da remoção de um mínimo de registos em falta e dos valores atípicos por truncamento aos limites inferior e superior.
- Remoção de variáveis redundantes (com correlação entre si superior a 0.90) e de variáveis com baixa variância (inferior a 0.10).
- Discretização da variável-alvo Receita_Total em 3 classes (Baixa, Média e Alta).
- Modelação: Avaliação de 2 modelos de clustering, K-Means e Aglomerativo Hierárquico.
- Análise de valores atípicos com o modelo Local Outlier Factor (LOF).
- Análise crítica de clusters e anomalias, com hipóteses para explicação de fenómenos atípicos.
________________________________________

## Resultados Principais

________________________________________

## Estrutura do Projeto
1. Perfilamento dos Dados: análise exploratória, valores omissos e atípicos, distribuições e correlações.
2. Pré-processamento dos Dados: tratamento de valores omissos e de valores atípicos, remoção de variáveis redundantes e de variáveis com baixa variância e discretização da variável-alvo.
3. Clustering: aplicação e avaliação dos modelos de K-Means e Aglomerativo Hierárquico com métricas internas (Índices de Silhueta, Inércia e de Davies-Bouldin) e métricas externas (Índices de Pureza e de Rand).
4. Análise de Valores Atípicos: deteção multivariada com LOF, análise bivariada de variáveis relevantes e estudo das pontuações de anomalia.
5. Avaliação Crítica: interpretação dos clusters, hipóteses para desvios, impacto do pré-processamento e análise de anomalias.
________________________________________

## Ferramentas Utilizadas
- Jupyter Notebook
- Python
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn
________________________________________

## Conteúdos do Repositório
- Jupyter Notebook - Projeto - Data Science e Análise Não-Supervisionada - Conjunto de Dados Cinema - Alexandre Vasconcelos.ipynb - Código do projeto
- Relatório PDF - Projeto - Data Science e Análise Não-Supervisionada - Conjunto de Dados Cinema - Alexandre Vasconcelos.pdf - Relatório do projeto, detalhado com a descrição e os resultados da análise
________________________________________

## Como Visualizar os Resultados
1. Clonar o repositório
2. Abrir no Jupyter Notebook o ficheiro `.ipynb`
3. Executar as células por ordem para reproduzir a análise
________________________________________

## Contactos
- Nome: Alexandre Vasconcelos
- Email: alex-0.5@hotmail.com
- LinkedIn: https://www.linkedin.com/in/alexandre-vasconcelos-396227167/
