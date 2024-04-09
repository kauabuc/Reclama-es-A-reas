# Reclamações Aéreas

### O projeto completo se encontra no meu [Medium](https://medium.com/@kakabuchweitz/melhoria-do-canal-de-atendimento-das-principais-companhias-a%C3%A9reas-do-brasil-1b3cd7d120f7)
### [Confira aqui o dashboard do projeto.](https://app.powerbi.com/view?r=eyJrIjoiNDA0OGIzNmItMzMxOS00MTY3LTlhNmUtNDI3M2NhYjk1MTg2IiwidCI6IjBjMzkwMzgzLTc1NTQtNDdkOC05YmVkLTgxMDI3YzBjMjE4OCJ9&pageName=ReportSection712922e69aabaa73e159)

### Overview do Projeto
---

O projeto apresenta uma análise, além de um plano de melhoria voltado para a área de atendimento ao cliente das três empresas mais influentes no Brasil (Azul, Gol e Latam), que continham mais números de viagens ao longo dos últimos anos.

No projeto, foi feito seguindo as normas e orientações da metodologia CRISP-DM.

### Limitações

Na análise inicial feita no Power BI, foi obtido que a base original (com dados de 2019 a 2022) contém 338 mil linhas e 38 colunas, entretanto o conjunto de dados que foi exportado para a análise contém 152 mil linhas e apenas as 3 principais empresas do ramo aéreo do Brasil, Azul, Gol e Latam. <br>
As demais linhas contavam com valores que o atendimento não foi avaliado ou não foi dado uma nota pelo atendimento. Sendo assim, essas linhas foram descartadas para um futuro estudo, com objetivo de entender o porquê do cliente não classificou seu atendimento, ficando disponível apenas se a reclamação foi resolvida ou não. <br> 

Assim ficamos com 152 mil linhas e apenas com dados classificados pelos clientes e referentes a alguma das três principais empresas.
Das 29 colunas, ela possui apenas 4 variáveis quantitativas, 3 variáveis do tipo data, 3 do tipo hora e 19 variáveis qualitativas.

### DATA

A Base de dados é formada por dados dos anos de 2019 a 2022, referente as reclamações registradas no canal do consumidor.gov que contabilizam o atendimento prestado por empresas aéreas ao consumidor.
O metadados da base e as bases se encontram no [Consumidor.gov](https://www.anac.gov.br/acesso-a-informacao/dados-abertos/areas-de-atuacao/voos-e-operacoes-aereas/dados-do-consumidor-gov).

### Ferramentas

- Python - Análise dos Dados
- PowerBI - Criação do relatório e acompanhamento dos indicadores


### Preparação dos Dados
As seguintes variáveis possuíam erro ou algum valor faltante nesse caso foi feito:
1. Sexo: 7 valores faltantes, preenchido com o valor que mais ocorre no conjunto, no caso "Masculino".
2. Na análise em Python foi necessário realizar uma transformação das colunas de Data e Hora que foram recebidas como objeto para seu valor original.
3. Criação da variável "Atendimento", baseado para resposta do negócio, se a nota do consumidor for acima ou igual a 4, é classificado como bom, caso contrário, ruim.
4. Criação da variável "Tempo para Finalizar", que indica o tempo que durou o atendimento prestado ao cliente.
5. Remoção de 90 linhas que ainda continham valores faltantes na base na coluna referente a Data da Finalização.


### Exploratory Data Analysis (Análise Exploratória dos Dados)

Ao longo da Análise, se baseou em perguntas chaves como critério de sucesso, que visavam a melhora do canal de atendimento: 

- Analisar quais as principais reclamações dos clientes em relação aos serviços prestados.
- Que áreas mais causam/geram insatisfação?
- Qual o nível de satisfação com o atendimento prestado?
- O que deve se priorizar para contornar o problema?

### Análise

Alguns dos insigths obtidos nessa etapa foram: 

1. 60% das reclamações vieram do sexo masculino.
2. De 31 a 40 anos foram onde tiveram mais ocorrências de reclamações.
3. A Latam predomina em reclamações no período.


### Resultados

Alguns dos resultados a serem comunicados:
1. Cerca de 55% das reclamações tiveram um bom atendimento de acordo com os clientes.
2. Entre os grupos do problema, os que mais ocorreram foram relativos a Cobrança, Contrato / Oferta e ao atendimento.
3. Referente a avaliação do consumidor, 71% das notas foram distribuídas em 5 (42%) ou em 1 (31%).

### Recomendações

Baseado na Análise podemos recomendar ações como:
![planodeação](https://github.com/kauabuc/ReclamacoesAereas/blob/main/gr%C3%A1ficos/planodeacao.jpg)

### Conclusão

Graças a análise, técnicas estatísticas e ferramentas utilizadas, foi possível gerar uma solução para a área de Atendimento.
A apresentação do projeto demostra e aponta uma visão geral do projeto de melhoria do atendimento das principais empresas aéreas do Brasil, alinhado com objetivos, estratégias, execução e recursos necessários par ao seu sucesso.


