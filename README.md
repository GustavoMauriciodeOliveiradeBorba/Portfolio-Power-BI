# Portfólio Power BI 

 Dashboards desenvolvidos com ênfase no aprendizado da ferramenta Power BI, com o objetivo de criar um portfólio que reflete situações cotidianas reais:



**Dashboard de Vendas, Custo, Margem de Lucro e KPI**


![DashboarddeVendasCustoMargemdeLucroeKPI-PowerBIemais4pginas-PessoalMicrosoftEdge2024-04-2816-32-48-ezgif com-video-to-gif-converter](https://github.com/GustavoMauriciodeOliveiradeBorba/Portfolio-Power-BI/assets/168369314/b2905e4c-4050-47a9-b138-e0010db894f9) 

Arquivo Cliente.csv que contém inicialmente as seguintes colunas:

**_Tabela Cliente_**
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


