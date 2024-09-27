# Criando-Dashboard-de-Vendas-com-PowerBI-Utilizando-Star-Schema
Quarto Desafio com Power BI - NTT DATA Bootcamp

## Descrição do desafio de modelagem dimensional
 - Objetivo: criar o diagrama dimensional – star schema – com base no diagrama relacional disponibilizado.
<div align="center">
  <img src="https://github.com/user-attachments/assets/bc485005-2314-46fa-80bb-53084233f653" height="450px" width="700px">
</div></br>

 - Foco: Professor (objeto de análise).  
  Montar o esquema em estrela com o foco na análise dos dados dos professores. Sendo assim, a tabela fato deve refletir diversos dados sobre professor, cursos ministrados, departamento ao qual faz parte...Já se têm uma ideia do que deve compor a tabela fato do modelo em questão.

   Obs.: Não é necessário refletir dados sobre os alunos!

- O que deve ser feito?
 Deverá ser criada a tabela Fato que contêm o contexto analisado. Da mesma forma, é necessária a criação das tabelas dimensão que serão compostas pelos detalhes relacionados ao contexto.
 Por fim, mas não menos importante, adicione uma tabela dimensão de datas. Para compensar a falta de dados de datas do modelo relacional, suponha que você tem acesso aos dados e crie os campos necessários para modelagem.
 Ex: data de oferta das disciplinas, data de oferta dos cursos, entre outros. O formato, ou melhor, a granularidade, não está fixada. Podem ser utilizados diferentes formatos que correspondem a diferentes níveis de granularidade.

# Descrição dos passos usados:

  1. Criação das tabelas e seus atributos no MySQLWorkbench;
  2. Importação do banco de dados para o Power BI Desktop;
  3. Em Modelagem, redução das entidades ao modelo Star Schema;
  4. Criação da Tabela Datas e adição de colunas:  
     (Obs.: DAX CALENDARAUTO([fiscal_year_end_month]), o fiscal_year_end_month = 1 semestre letivo);
  6. Hierarquização conforme a granularidade;
  7. Substituição da Tabela Alunos por Datas;
  8. Relacionamento entre as entidades, conforme o Star Schema;
