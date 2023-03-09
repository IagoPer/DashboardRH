# DashboardRH:zap:

### Dashboard de RH em Power BI

O Dashboard abaixo refere-se a uma base de RH contendo informações de funcionários, áreas, cargos e salários. Nele é apresentado informações do total de Contratações, Demissões, Funcionários Ativos, Percentual de TurnOver, Quantidade de Funcionários por Cidade, Gênero, Cargo e Setor.

No primeiro momento foi necessário realizar algumas alterações no Power Query, sendo essas o tipo de cada coluna, limpeza de dados desnecessários, desmembramento da base para criação de tabelas de dimensão afim de diminuir a quantidade de dados/informações repetitivas e melhorar o desempenho do Dashboard. Automaticamente, com o desmembramento da base foi necessário realizar o gerenciamento das relações entre a tabela fato e suas dimensões:

<img width="425" alt="Relacionamentos" src="https://user-images.githubusercontent.com/98985401/224115929-b13a2b46-6835-4455-9224-24af47455819.png">

Em seguida, foram criadas as medidas para cálculo da quantidade de contratação, demissão, funcionários ativos, horas extras e turnover:

<img width="128" alt="Medidas" src="https://user-images.githubusercontent.com/98985401/224116100-0ad60060-d311-430f-97e7-e701a3a9b505.png">

No layout, foi usado o Sparkline by OKViz para apresentar a evolução das contratações no decorrer do tempo. Cartões para apresentar o total de Contratações, Funcionários Ativos, Demissões e TurnOver. Funil para visualização da quantidade de funcionários em cada estado atrelado a uma Tooltip contendo informações do total de hora extra, funcionários ativos e salário. Gráfico de Rosca contendo o percentual para o gênero dos funcionários. E por fim, uma Árvore Hierárquica contendo o total de funcionários ativos distribuídos por setor e cargo:

<img width="425" alt="Dash1" src="https://user-images.githubusercontent.com/98985401/224116412-b7890484-aa57-475d-848f-42da09dc5953.png">

<img width="425" alt="Dash2" src="https://user-images.githubusercontent.com/98985401/224116440-0ea52d67-1e30-41cb-b063-15d133c3aef3.png">

Diante das informações apresentadas podemos gerar os seguintes Insights:

  :heavy_check_mark:	Há um total de 234 contratações;

  :heavy_check_mark: 217 são funcionários ativos;

  :heavy_check_mark: Houve 17 demissões ao longo do tempo;

  :heavy_check_mark: A taxa de TurnOver é de 7,26%;

  :heavy_check_mark: O estado que detém maior número de funcionários ativos é São Paulo;

  :heavy_check_mark: No estado de São Paulo o cargo com maior quantidade de horas extras são os estagiários;
  
  :heavy_check_mark: O setor que detém maior número de funcionários ativos é o Administrativo.

Esses Insights são de grande valia, pois por meio deles podemos nos aprofundar nas informações identificando pontos que precisam de atenção, como por exemplo:

  :heavy_check_mark: A quantidade/realização de horas extras por estagiários;
  
  :heavy_check_mark: Cargos e salários são equivalentes em todos os estados;
  
  :heavy_check_mark: Estudo de caso e plano de meta para igualar o percentual de funcionários do gênero femino e masculino.
