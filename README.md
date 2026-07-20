# SCTEC-PROJETO_02

Análise de Dados de Recursos Humanos
Autora: Camilla Nascimento de Oliveira
Curso:  Visualização de Dados e Business Intelligence [T2]  
Módulo: Módulo  1 
Projeto: Projeto Avaliativo 2

1.	Sobre o projeto
Este projeto foi desenvolvido com o objetivo de analisar dados de Recursos Humanos utilizando SQL e Python. No caso em questão, utilizei o google colab para poder ter acesso às bibliotecas e fazer a análise exploratória dos dados.
A análise foi realizada a partir de dados relacionados a funcionários, cargos, departamentos, salários e localização geográfica (país, cidade).

2.	O projeto foi desenvolvido seguindo o fluxo
Consultas SQL
      
Exportação dos resultados para CSV
      
Análise exploratória com Python
      
Tratamento dos dados
      
Estatística descritiva
      
Visualizações
      
Identificação de insights

3.	Objetivo
O objetivo deste projeto é analisar a estrutura salarial dos funcionários e identificar possíveis padrões relacionados a cargos, departamentos e regiões.
A análise busca responder às seguintes perguntas:
•	Como os salários estão distribuídos? 
•	Qual é a média salarial dos funcionários? 
•	Existem diferenças significativas entre os salários? 
•	Quais departamentos apresentam maiores salários médios? 
•	Como o salário médio dos principais cargos se posiciona em relação às faixas salariais mínima e máxima? 
•	Existem valores salariais potencialmente discrepantes?

4.	Base de dados
A análise foi realizada utilizando dados do esquema HR (Human Resources) do FreeSQL. As consultas utilizaram informações relacionadas às seguintes informações:
•	Funcionários; 
•	Departamentos; 
•	Cargos; 
•	Localizações; 
•	Países; 
•	Salários;
•	Regiões.

5.	Principais informações utilizadas
Funcionários
•	Identificação do funcionário; 
•	Nome e sobrenome; 
•	Salário; 
•	Departamento; 
•	Cargo. 
Cargos
•	Nome do cargo; 
•	Salário mínimo; 
•	Salário máximo. 
Localização
•	Cidade; 
•	Estado ou província; 
•	País; 
•	Região.

6.	Consultas SQL
Query_01 — Análise salarial por cargo e departamento
A primeira consulta relaciona os funcionários aos seus respectivos cargos e departamentos. Foram utilizadas informações como:
•	identificação do funcionário; 
•	nome do funcionário; 
•	salário; 
•	departamento; 
•	cargo; 
•	salário mínimo do cargo; 
•	salário máximo do cargo. 
Essa consulta permitiu realizar análises relacionadas à:
•	distribuição salarial por cargo/função; 
•	média salarial;
•	mediana salarial;
•	mínimo e máximo salarial; 
•	comparação entre os cargos; 
•	comparação entre salário médio e faixa salarial dos cargos. 
O arquivo utilizado foi - query_01.csv.

7.	Query_02 — Análise salarial por região
A segunda consulta relaciona os funcionários às informações de localização geográfica. Foram utilizadas informações como:
•	identificação do funcionário; 
•	nome; 
•	salário; 
•	departamento; 
•	cidade; 
•	estado ou província; 
•	país; 
•	região. 
Essa consulta permitiu analisar a distribuição dos funcionários e dos salários considerando a localização geográfica.

8.	Análise exploratória em Google Colab (Python)
Os resultados das consultas SQL foram exportados para arquivos CSV e posteriormente analisados utilizando Google Colab. As bibliotecas utilizadas foram:
•	Pandas; 
•	Matplotlib; 
•	Seaborn. 
Durante a análise exploratória foram realizadas as seguintes etapas:
•	carregamento dos arquivos CSV; 
•	inspeção inicial dos dados; 
•	análise da estrutura dos DataFrames; 
•	verificação dos tipos de dados; 
•	identificação de valores ausentes; 
•	verificação de duplicatas; 
•	tratamento dos dados; 
•	conversão dos salários para formato numérico; 
•	cálculo de estatísticas descritivas; 
•	agrupamento dos dados por departamento; 
•	análise dos cargos com maiores salários médios; 
•	comparação entre salário médio e faixa salarial dos cargos; 
•	criação de visualizações gráficas – gráficos em barras e gráfico de dispersão.

9.	Estatística descritiva
A análise da variável SALARY apresentou os seguintes resultados:
Medida	Resultado
Média	$ 6.456,75
Mediana	$ 6.150,00
Mínimo	$ 2.100,00
Máximo	$ 24.000,00
Desvio padrão	$ 3.927,80
A média salarial foi superior à mediana, indicando que salários mais elevados influenciam a distribuição dos dados. A diferença entre a média e a mediana sugere uma distribuição assimétrica, com a presença de salários mais altos que elevam a média geral. O desvio padrão também demonstra uma dispersão significativa dos salários em relação à média.

10.	Visualizações
O painel final reúne quatro análises principais:
1.	Distribuição dos salários; 
2.	Distribuição e identificação de possíveis outliers; 
3.	Média salarial por departamento; 
4.	Comparação entre salário médio e faixa salarial dos principais cargos. 
a)	Distribuição dos salários
O histograma permite visualizar a concentração dos salários e compreender como os valores estão distribuídos entre os funcionários.
b)	Distribuição e possíveis outliers
O boxplot permite analisar a dispersão dos salários e identificar valores que podem estar distantes da distribuição central. Esses valores não devem ser automaticamente considerados erros. Eles podem representar cargos de maior responsabilidade ou posições hierárquicas superiores.
c)	Média salarial por departamento
A comparação entre as médias salariais dos departamentos permite identificar diferenças na remuneração média entre as áreas da organização.
d)	Salário médio e faixa salarial dos principais cargos
A comparação entre o salário médio e os valores mínimo e máximo previstos para os principais cargos permite observar a posição da remuneração média dentro da faixa salarial de cada cargo. Essa análise permite identificar cargos cujo salário médio está mais próximo do limite inferior ou superior da faixa salarial.

11.	Principais insights
A análise permitiu observar que:
•	os salários apresentam dispersão significativa; 
•	a média salarial é superior à mediana; 
•	existem salários elevados que influenciam a média geral; 
•	há diferenças de remuneração média entre os departamentos; 
•	os cargos apresentam diferentes faixas salariais; 
•	a comparação entre salário médio e faixa salarial permite compreender melhor a distribuição da remuneração; 
•	a análise conjunta de cargo, departamento e salário permite uma visão mais ampla da estrutura de remuneração da organização.

12.	Possibilidades de análises futuras
Como evolução da análise, poderiam ser desenvolvidos estudos adicionais, como:
•	análise da relação entre salário e tempo de empresa; 
•	comparação entre funcionários recém-contratados e funcionários mais antigos; 
•	análise de evolução salarial ao longo do tempo; 
•	análise de salários por nível de senioridade; 
•	identificação de cargos com maior diferença entre salário médio e faixa salarial; 
•	comparação entre a faixa salarial dos cargos e dados de mercado; 
•	análise da adequação da faixa salarial para novas contratações; 
•	criação de um dashboard interativo para acompanhamento dos indicadores de Recursos Humanos.

Tecnologias utilizadas
•	SQL; 
•	Pandas; 
•	Matplotlib; 
•	Seaborn; 
•	GitHub; 
•	Google Colab.
