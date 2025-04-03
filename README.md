# Desafio Clustering
Desafio apresentado como requisito para a formação no curso de Cientista de Dados pela Escola DNC. 

Foram utilizadas majoritariamente as bibliotecas Pandas e SKLearn, bem como outras auxiliares. Foi feito todo o tratamento dos dados, como remoção de dados nulos e análise dos outliers e em sequência, foram testados alguns métodos de clustering mais populares. Ao final do desafio, foi realizada uma análise de cada cluster de cliente e, com base nisso, sugerida uma estratégia a ser seguida pela empresa.

## Tecnologias Utilizadas
<div <br> 
<img src="https://img.shields.io/badge/Python-4695dd?style=for-the-badge&logo=python&logoColor=FFD43B">
<img src="https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white">
<img src="https://img.shields.io/badge/scikitlearn-F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white">
<img src="https://img.shields.io/badge/Matplotlib-%232A9D8F.svg?style=for-the-badge&logo=Matplotlib&logoColor=black"
</div> 
  
## Proposta
### Crie um modelo de análise das métricas RFV
Você foi contratado por uma empresa de e-commerce que está buscando entender melhor o comportamento de seus clientes para personalizar as suas campanhas de marketing. Para isso, a empresa disponibilizou uma base de dados em csv contendo dados sobre clientes, produtos e transações da loja realizadas entre os anos de 2010 e 2011.

Com base nesses dados, você precisa agrupar os clientes em clusters com base em seu comportamento de compra. Isso irá permitir identificar padrões e características em comum entre os clientes, como:

- Clientes que compram os mesmos produtos;
- Clientes que possuem a mesma frequência de compras;
- Clientes que gastam mais dinheiro em suas compras.

A partir desses clusters, gere insights para que a empresa possa segmentar melhor a sua base de clientes e personalizar as suas campanhas de marketing, direcionando promoções e ofertas aos clientes com base no comportamento de compras.

## Conclusão
Com base nas análises realizadas, foram encontrados 4 grupos de clientes bem distintos:
<p align="center">
  <img src="https://github.com/user-attachments/assets/fa78b1d5-8c90-4010-b856-35d4a1927d7f" 
  alt="Tabela RFM para cada cluster">
</p>

1. Clientes deste cluster são os mais recentes e frequentes. Eles compram regularmente e têm um gasto médio razoável. Estes clientes podem ser considerados fiéis, que fazem compras repetidas e têm um bom histórico de gastos.
2. Este grupo de clientes fez compras há algum tempo (cerca de 1 mês e meio atrás), mas tem uma frequência mais baixa de compras. O gasto médio também é um pouco menor, mas ainda substancial. Esses clientes podem estar em um estágio intermediário: não são recentes, mas também não estão completamente inativos.
3. Este grupo de clientes fez compras ainda mais distantes, com uma frequência também moderada. No entanto, eles se destacam por gastar mais por compra, o que pode indicar que são clientes menos frequentes, mas que compram em maiores quantidades. Eles são um grupo importante devido ao seu alto valor monetário.
4. Este cluster representa clientes inativos há muito tempo (mais de 8 meses). A frequência de compras é muito baixa, e o gasto também é relativamente baixo. Esses clientes podem ser considerados como clientes em risco de abandono, churned, ou clientes esporádicos, que não geraram compras recentes e provavelmente não estão muito envolvidos com a marca.

Com isso, pode ser elaborada uma estratégia baseada em cada grupo individualmente, ou conforme a empresa desejar. Por exemplo, os grupos 2 e 3 representam clientes em risco, que não compram com tanta frequência quanto o primeiro grupo. Assim, campanhas de reativação, como ofertas especiais ou lembretes de produtos, podem ser direcionadas para tentar trazer esses clientes de volta. Ainda, o grupo 2 tem um alto gasto médio, o que indica que, mesmo com baixa frequência, eles podem ser clientes importantes para a marca. Estratégias de up-selling ou cross-selling podem ser eficazes, oferecendo produtos complementares de alto valor.
