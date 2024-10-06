### ==Convidado: [@MarcLamberti](https://www.linkedin.com/in/marclamberti/)==

## Por que usar Airflow?
Para facilitar e ganhar tempo no desenvolvimento de *pipelines* de dados.

## O que vamos construir
### Uma solução moderna de dados do zero
* Utilizando principalmente **SQL**
* Integrando dados com **Airbyte**
* Transformando os KPIs com **DBT-Core**
* Orquestrando tudo com **Aitflow**
![[Pasted image 20241005213521.png]]
### O que buscamos com uma Modern Data Stack?
* Majoritariamente utilizando **SQL**
* Foco na velocidade de entrega, sem perder qualidade
* O mesmo profissional ser capaz de criar solução completa end-to-end
* Grande foco na área de negócio
## Exemplo de problema
### Eficiência de Campanha:
* Custo por Clique (CPC): `Total de gastos / Total de cliques`
* Custo por Impressão (CPM): `( Total de gastos / Total de impressões ) * 1.000`
* Custo por Lead (CPL): `Total de gastos / Total de leads gerados`
### Eficácia de Campanha:
* Taxa de Conversão de Cliques: `Total de leads gerados / Total de cliques`
* Taxa de Engajamento: `( Total de eventos engajados / Total de sessões ) * 100`
### Performance de Conteúdo:
* Alcance por Impressão `Total de alcance / Total de impressões`
* Relação Engajamento/Alcance: `Total de eventos engajados / Total de alcance`
### Retorno sobre Investimento (ROI)
## Como podemos fazer análise isoladas
- Google Analytics 4
- META ads
- SalesForce
- Excel
- Google Sheets
- Pentaho
- Supermetrics
- **==Airbyte==**
## [Airbyte](https://airbyte.com/)
Ele basicamente serve para integrar os sistemas
![[Pasted image 20241005215951.png]]
1. Conectando nossas fontes (**Configurar Source**)
	- Google Analytics
	- Facebook Ads
	- Planilhas (Pesquisa)
1. Conectando nossos destinos (**Configurar Destinations**)
	- PostgresSQL (hosted on **==Render==**)
2. Criando nossas conexões (**Configurar Connections**)
	- Source $\rightarrow$ Destino