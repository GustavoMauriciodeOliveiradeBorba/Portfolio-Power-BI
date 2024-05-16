# Portfólio Power BI 

 Dashboards desenvolvidos com ênfase no aprendizado da ferramenta Power BI, com o objetivo de criar um portfólio que reflete situações cotidianas reais:

- [Dashboard de Vendas, Custo, Margem de Lucro e KPI](https://github.com/GustavoMauriciodeOliveiradeBorba/Portfolio-Power-BI/tree/8935b461aa95ccf739cd7cf37ce9623d73b5e181/Dashboard%20de%20Vendas%2C%20Custo%2C%20Margem%20de%20Lucro%20e%20KPI)
- [Dashboard Analítico de Vendas Globais](https://github.com/GustavoMauriciodeOliveiradeBorba/Portfolio-Power-BI/tree/8935b461aa95ccf739cd7cf37ce9623d73b5e181/Dashboard%20Anal%C3%ADtico%20de%20Vendas%20Globais)
- [Dashboard Análise Financeira](https://github.com/GustavoMauriciodeOliveiradeBorba/Portfolio-Power-BI/tree/c8176a05cbf9183c99eadd90f7994e077e88fa91/Dashboard%20An%C3%A1lise%20Financeira)

**Dashboard de Vendas, Custo, Margem de Lucro e KPI**


![DashboarddeVendasCustoMargemdeLucroeKPI-PowerBIemais4pginas-PessoalMicrosoftEdge2024-04-2816-32-48-ezgif com-video-to-gif-converter](https://github.com/GustavoMauriciodeOliveiradeBorba/Portfolio-Power-BI/assets/168369314/b2905e4c-4050-47a9-b138-e0010db894f9) 

**Contexto para a criação do Dashboard**
|Tente responderas perguntas no Power BI construindo os gráficos:|
| --- | 
|1-Qual foi o total de valor venda considerando cada modo de envio dos pedidos? Use um gráfico de cascata.|
|2-Quais mercados tiveram o maior custo médio de envio dos produtos vendidos? Use um gráfico treemap.|
|3-A empresa tem como objetivo (meta) manter uma média de 350 para o valor de venda todos os meses. Mostre um indicador (KPI–Key Performance Indicator) com o valor médio de venda. A empresa ficou abaixo ou acima da meta no mês de Abril/2014?|
|4-Considere que o lucro é equivalente a:valor venda -custo envio. Qual categoria de produto apresentou maior lucro médio.|
|5-Qual foi o comportamento da margem de lucro ao longo do tempo? Considere amargem de lucro como o lucro dividido pelo valor venda.|

**_Bases de dados utilizadas_**

 Para a criação deste dashboard, foram utilizadas 4 fontes de dados, sendo elas:

 - Clientes.csv
 - Pedidos.csv
 - Produtos.csv
 - Vendas.csv

_Observação: Apenas a tabela vendas ganhou colunas adicionais, conforme descrição a seguir:_

Arquivo Vendas.csv que contém inicialmente as seguintes colunas:

**Tabela Vendas**
- Pedido;
- Cliente;
- Produto;
- Valor Venda;
- Quantidade vendida;
- Custo Envio.
  
**_Colunas criadas a partir dos dados:_**
  - Lucro;
  - Margem de Lucro.

**_Fórmula dax utilizada para criação da coluna lucro:_**

> **Lucro = Vendas[Valor Venda] - Vendas[Custo Envio]**

**_Fórmula dax utilizada para criação da coluna Margem Lucro:_**

> **Margem Lucro = ROUND(DIVIDE(Vendas[Lucro],Vendas[Valor Venda]) * 100,2)**

**Relacionamento entre as tabelas**

Todos os relacionamentos criados, utilizaram a cardinalidade Muitos para Um (*:1)

![image](https://github.com/GustavoMauriciodeOliveiradeBorba/Portfolio-Power-BI/assets/168369314/49786ffb-ef89-4ca7-9b84-787e071dfa32)


**Dashboard Analítico de Vendas Globais**

![DashboardAnalticodeVendasGlobais-PowerBI-PessoalMicrosoftEdge2024-05-1516-14-06-ezgif com-video-to-gif-converter](https://github.com/GustavoMauriciodeOliveiradeBorba/Portfolio-Power-BI/assets/168369314/5641fff4-b9c4-4beb-8429-df1b0871d26d)


**Contexto para a criação do Dashboard**

|Nosso Dashboard deve responder as perguntas abaixo:|
| --- | 
|•Pergunta 1 -Qual o valor total vendido?|
|•Pergunta 2 -Quantas vendas foram realizadas por categoria de produto?|
|•Pergunta 3 -Quantas vendas foram realizadas por país considerando a prioridade de entrega?|
|•Pergunta 4 -Qual foi o percentual de desconto nas vendas por subcategoria de produto?|
|•Pergunta 5 -Quais países tiveram maior média de valor de venda? Demonstre em um mapa.|


**_Composição da Bases de dado utilizada_**

 Para a criação deste dashboard, foi utilizada apenas uma fonte de dados:

- Dataset.csv

Arquivo Dataset.csv que contém inicialmente as seguintes colunas:
- ID_Pedido;
- Data_Pedido;
- ID_Cliente;
- Segmento;
- Regiao;
- Pais;
- Product ID;
- Categoria;
- SubCategoria;
- Total_Vendas;
- Quantidade;
- Desconto;
- Lucro;
- Prioridade

  Nenhuma coluna adicional foi criada.


  **Dashboard Análise Financeira**

![AnlisedeDadosFinanceiros-PowerBIemais2pginas-PessoalMicrosoftEdge2024-05-1519-56-30-ezgif com-video-to-gif-converter](https://github.com/GustavoMauriciodeOliveiradeBorba/Portfolio-Power-BI/assets/168369314/6edb1027-ae8f-4e8e-8e9e-86927e163a3d)

**Contexto para a criação do Dashboard**

| Criar um Dashboard que permita analisaros seguintes indicadores financeiros: |
| --- | 
|1-Total de Receitas;|
|2-Total de Despesas;|
|3-Margem de Lucro;|
|4-Total de ReceitasPor Componente;|
|5-Total de Despesas Por Componenteem relação à média de Despesas;|
|6-Total  de  Receitase  DespesasPor  Componente  e  Por  Ano,com  a  hierarquia Tipo/Componente.|
|Além disso identificar os segmentos onde Receitas e Despesas são maiores e menores a fim de traçar seu plano estratégico.|


**_Composição da Bases de dado utilizada_**

   Para a criação deste dashboard, foi utilizada apenas uma fonte de dados:
   
  -DadosFinanceiro.xlsx

  Arquivo DadosFinanceiro.xlsx que contém inicialmente as seguintes colunas:
- Componente;
- Data;
- Tipo;
- Valor.

Com base nestes dados, foi criada a tabela de **MedidasindicadoresFinanceiros**, contendo as seguintes medidas:

- **Lucro**;
- **MargemLucro**;
- **TotalDespesas**;
- **TotalReceitas**

**_Fórmula dax utilizada para criação da medida lucro:_**
>**Lucro = [TotalReceitas] - [TotalDespesas]**
  
**_Fórmula dax utilizada para criação da medida MargemLucro:_**
>**MargemLucro = DIVIDE([Lucro],[TotalReceitas] , 0)**

**_Fórmula dax utilizada para criação da medida TotalDespesas:_**
>**TotalDespesas = CALCULATE(SUM(DadosFinanceiros[Valor]), DadosFinanceiros[Tipo] = "Despesas") **

**_Fórmula dax utilizada para criação da medida TotalReceitas:_**
>**TotalReceitas = CALCULATE(SUM(DadosFinanceiros[Valor]), DadosFinanceiros[Tipo]="Receitas")**



