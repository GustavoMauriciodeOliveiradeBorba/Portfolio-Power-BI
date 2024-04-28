# Portfólio Power BI 

 Dashboards desenvolvidos com ênfase no aprendizado da ferramenta Power BI, com o objetivo de criar um portfólio que reflete situações cotidianas reais:

- [Dashboard de Vendas, Custo, Margem de Lucro e KPI](https://github.com/GustavoMauriciodeOliveiradeBorba/Portfolio-Power-BI/tree/5db886b69a2b4e339a8c0133f0233eb7556c3aca/Dashboard%20Anal%C3%ADtico%20de%20Vendas%20Globais)

**Dashboard de Vendas, Custo, Margem de Lucro e KPI**


![DashboarddeVendasCustoMargemdeLucroeKPI-PowerBIemais4pginas-PessoalMicrosoftEdge2024-04-2816-32-48-ezgif com-video-to-gif-converter](https://github.com/GustavoMauriciodeOliveiradeBorba/Portfolio-Power-BI/assets/168369314/b2905e4c-4050-47a9-b138-e0010db894f9) 

**_Composição das Bases de dados utilizadas_**
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





