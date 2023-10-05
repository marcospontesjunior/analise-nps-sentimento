# Análise de Produto: Integrando NPS e Análise de Sentimento

###
[![License: MIT](https://img.shields.io/badge/License-MIT-black.svg)](https://opensource.org/licenses/MIT) 

### Sobre:

O objetivo deste projeto é realizar uma análise da base de dados para calcular o Net Promoter Score (NPS) e utilizar a API do ChatGPT para realizar uma análise de sentimento.

### Proposta:

A proposta do projeto é aplicar uma abordagem analítica que nos permita compreender a percepção e a experiência dos clientes de forma aprofundada. Utilizando uma API para análise de sentimento para extrair informações dos feedbacks, identificando padrões e tendências que nos ajudarão a tomar decisões estratégicas com base nas opiniões dos clientes.

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

Uma empresa especializada em cosméticos para cuidados masculinos solicitou a realização de uma análise de NPS (Net Promoter Score) e de sentimento em relação ao seu produto, um óleo para barba.

Inicialmente, utilizamos a biblioteca **Pandas** para importar e ler a base de dados.

<img src="/img/dados.png">

###
Em seguida, criamos um gráfico para compreender a distribuição da quantidade de notas nas categorias Detratores, Passivos e Promotores.

<img src="/img/grafico_notas.png">

###
Utilizamos um laço **for** para calcular o NPS com base nas notas dadas pelos consumidores, resultando em um valor aproximado de **29,29** no cálculo do NPS.

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
```

###
O próximo passo foi criar um gráfico para contextualizar o valor obtido na escala do NPS.

<img src="/img/grafico_nps.png">

###
Concluímos a análise, identificando que o valor se encontra na faixa indicada como **'Aperfeiçoamento'** na escala do NPS.

### Análise de Sentimento:

Utilizando a API do ChatGPT para realizar uma análise dos comentários do produto, obtivemos os resultados a seguir:

- A maioria dos comentários (66%) avalia o óleo de barba de forma positiva, com notas entre 7 e 10. Os aspectos mais elogiados são a maciez da barba, o brilho que proporciona e a hidratação duradoura.

- Alguns comentários mencionam especificamente o aroma agradável do óleo de barba, o que é considerado um fator positivo.

- Alguns usuários expressaram insatisfação com o produto (10% dos comentários), mencionando problemas como irritação na pele ou falta de atendimento às expectativas.

- Há comentários em que os usuários consideram o óleo de barba bom, mas apontam alguns aspectos que poderiam ser aprimorados, como a fragrância, o preço ou a embalagem.

### Conclusão:

Em geral, a análise indica uma resposta positiva ao óleo de barba, com a maioria dos usuários satisfeitos com a maciez, brilho e hidratação proporcionados. No entanto, é importante notar que alguns consumidores expressaram insatisfação relacionada a aspectos como irritação na pele e preço do produto. Além disso, foram identificadas sugestões de melhoria, especialmente em relação à fragrância, ao preço e à embalagem do óleo para barba.

Essas análises ofereceram insights para orientar decisões estratégicas futuras, visando aprimorar tanto o produto quanto a experiência dos consumidores. A contínua atenção a esses aspectos pode contribuir para a fidelização dos clientes e o sucesso a longo prazo.

---
### Contato:

<div>
  <a href="https://linkedin.com/in/marcospontesjunior" target="_blank"><img src="https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white&color=black" target="_blank"></a>  
  <a href = "mailto:marcospntsjunior@gmail.com"><img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white&color=black" target="_blank"></a>
</div>
