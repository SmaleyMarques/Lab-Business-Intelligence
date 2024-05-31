# **Projeto: Laboratório de Business Intelligence (SQL Server)**

## **Stack**
MS SQL Server, Talend, Power BI, MS Excel e Figma

## **Sobre**
Projeto de Laboratório de BI desenvolvido utilizando o Microsoft SQL Server como base de dados afim  de implementar um data warehouse para a consolidação dos dados que surge a partir da necessidade de gerar analise de performance de vendas neste caso fictício, através da automação de um processo de ETL com a ferramenta Talend, deixando os dados , disponíveis para serem consumidos no Power BI. Projeto minuciosamente documentado no Microsoft Excel, relatórios comerciais desenvolvidos e apresentados de forma intuitiva e interativa no Power BI.

Todo o projeto, incluindo modelagem, códigos e scripts, está disponível no repositório, proporcionando acesso completo e detalhado. O DDL do data warehouse e os artefatos de ETL estão documentados para facilitar a compreensão e colaboração.

## **Descrição do Case**
Uma loja de artigos esportivos e suprimentos voltados para ciclismo deseja analisar seus dados de vendas. A loja possui um sistema ERP que armazena os dados em um banco de dados OLTP no MS SQL Server. Para a análise dos dados, foi criado um banco de dados OLAP, também no MS SQL Server, através de um processo ETL realizado com o Talend. Nesse processo, foram desenvolvidos jobs para extrair do banco de dados OLTP para o OLAP as tabelas de staging, que apoiam o processo de ETL, além das tabelas de dimensões e tabelas de fatos necessárias para a análise dos dados. Esses jobs são agendados para serem executados diariamente, garantindo que o banco de dados OLAP esteja sempre atualizado. Esse dataset é importado e consumido no Power BI, onde as tabelas foram devidamente relacionadas para a criação de medidas e visuais em um dashboard intuitivo e interativo.

## **Sobre os Dados Armazenados**
Os dados são fictícios, criados manualmente e com revisões e ajustes para a consistência de dados.

## **Mapa Geral do Projeto**
![Mapa Geral](https://github.com/SmaleyMarques/Lab-Business-Intelligence/blob/main/misc/ProjetoBI_mindmap.png)

## **Processo de Staging**
![staging](https://github.com/SmaleyMarques/Lab-Business-Intelligence/blob/main/misc/Staging.png)

## **Carga das Tabelas Dimensão**
![Dimensões](https://github.com/SmaleyMarques/Lab-Business-Intelligence/blob/main/misc/Dimens%C3%B5es.png)

## **Carga das Tabelas Fato**
![Fatos](https://github.com/SmaleyMarques/Lab-Business-Intelligence/blob/main/misc/Fatos.png)

## **Trucante Staging**
![Truncates](https://github.com/SmaleyMarques/Lab-Business-Intelligence/blob/main/misc/Truncates.png)

## **Fluxo das Jobs**
O fluxo das jobs segue a ordem hierárquica das tabelas, respeitando as dependências entre elas e a criação de chaves surrogate.

### **Jobs Staging**
![JOBS_STAGING](https://github.com/SmaleyMarques/Lab-Business-Intelligence/blob/main/misc/JOBs_STAGING.png)

### **Jobs de Carga das Tabelas Dimensão**
![JOBs_DIM](https://github.com/SmaleyMarques/Lab-Business-Intelligence/blob/main/misc/JOBs_DIM.png)

### **Jobs de Carga das Tabelas Fato**
![JOBs_FATO](https://github.com/SmaleyMarques/Lab-Business-Intelligence/blob/main/misc/JOBs_FATO.png)

### **Jobs de Organização Geral**
![JOB_GERAL](https://github.com/SmaleyMarques/Lab-Business-Intelligence/blob/main/misc/JOB_GERAL.png)

## **Modelagem dos dados no PowerBI**
![modelagem](https://github.com/SmaleyMarques/Lab-Business-Intelligence/blob/main/misc/modelagem.png)

## **Design no Figma**
Para melhorar a visualização e a estilização dos dashboards, foi desenvolvido um design de apoio no Figma, utilizando uma paleta de cores e elementos que se alinham com a identidade visual da loja (caso exista).

### **Aba Principal**
![BG - Painel Comercial](https://github.com/SmaleyMarques/Lab-Business-Intelligence/blob/main/misc/BG%20-%20Painel%20Comercial.png)

### **Aba de Análise**
![BG - Análise de Tendência](https://github.com/SmaleyMarques/Lab-Business-Intelligence/blob/main/misc/BG%20-%20An%C3%A1lise%20de%20Tend%C3%AAncia.png)

## **PowerBI**
Por fim, foram realizadas algumas análises utilizando o Power BI como ferramenta de visualização para criação do dashboard. Você pode acessar o dashboard interativo clicando [aqui](https://app.powerbi.com/view?r=eyJrIjoiMGFiYzQ4MDgtNjc3MC00N2I0LTkwNDgtYzU1NDhkNmFlNzY3IiwidCI6ImFiOGFiMGMyLTQ4ZTYtNDQ4Yy04YWJkLTk1MWViYzgxYjk0NCJ9)

![dashboard](https://github.com/SmaleyMarques/Lab-Business-Intelligence/blob/main/misc/dashboard.png)



