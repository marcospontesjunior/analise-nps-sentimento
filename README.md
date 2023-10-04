# Análise de NPS e Sentimento utilizando API do ChatGPT

###
[![License: MIT](https://img.shields.io/badge/License-MIT-black.svg)](https://opensource.org/licenses/MIT) 

### Sobre:

Este projeto tem como objetivo realizar uma análise da base de dados para calcular o Net Promoter Score (NPS) e, utilizar a API do ChatGPT para realizar uma análise de sentimento.

### Proposta:

A proposta do projeto é e aplicar uma abordagem analítica que nos permita compreender a percepção e a experiência dos clientes de forma aprofundada. Utilizando uma API para análisar sentimento para extrair informações qualitativas dos feedbacks, identificando padrões e tendências que nos ajudarão a tomar decisões estratégicas com base nas opiniões dos clientes.

### Estrutura do Repositório:
- <strong>data:</strong> Encontrará o arquivo **.csv** com os dados utilizados para a análise.
- <strong>img:</strong> Aqui você encontrará os prints obtidos na análise.
- <strong>notebook:</strong> Este diretório contém o notebook Jupyter onde a análise foi realizada e os resultados obtidos.
- <strong>readme_translated:</strong> This repository contains the **PDF** with the **report** translated into English.

### Linguagem Utilizada:
###
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=white&color=black)

### Bibliotecas Utilizadas:
###
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white&color=black) 	![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white&color=black) ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=white&color=black) ![OpenAI](https://img.shields.io/badge/OpenAI-%233F4F75.svg?style=for-the-badge&logoColor=white&color=black)

### Metodologia:

Uma empresa especializada em cosméticos para cuidados masculinos solicitou a realização de uma análise de NPS (Net Promoter Score) e de sentimento em relação ao seu produto, um óleo para barba. O objetivo é compreender a satisfação e a percepção dos consumidores em relação a esse produto específico, identificando pontos fortes e oportunidades de melhoria. 

Inicialmente, utilizamos a biblioteca **Pandas** para importar e ler a base de dados.

<img src=" ">

###
Criamos um gráfico para compreender a distribuição da quantidade de votos nas categorias Detratores, Passivos e Promotores.

<img src=" ">

###
Utilizamos um laço **for** para calcular o NPS com base nas notas dadas pelos consumidores.

```
nota = dados['nota']

detratores = 0
promotores = 0

for nota in notas:
  if nota >= 9:
    promotores += 1
  elif nota <= 6:
    detratores += 1

nps = (promotores - detratores) / len(notas) * 100

print(nps)
```

###
O valor obtido foi aproximadamente 29.29 no cálculo do NPS.

O próximo passo foi criar um gráfico para contextualizar o valor obtido na escala do NPS.

<img src=" ">

###
Concluímos a análise, identificando que o valor do NPS se encontra na faixa indicada como 'Aperfeiçoamento' na escala do NPS. Esta informação proporciona insights para orientar estratégias de aprimoramento do produto e do relacionamento com os consumidores.
