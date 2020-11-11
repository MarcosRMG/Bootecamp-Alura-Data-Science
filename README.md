# Bootecamp Alura Data Science

## Módulo 1: Analisando dados da saúde com Python e Pandas
### Aquisição e leitura de dados reais
Foram lidos três arquivos baixados no site do DATASUS (https://datasus.saude.gov.br/) para visualização dos custos de produção hospotalar. 
Inicialmente foi feita a visualização dos dados em tabela e por meio de um gráfico de linhas para entender como os dados estavam dispostos.

### Primeiras visualizações
Nas primeiras visualizações foram filtradas as colunas com dados válidos, excluíndo as colunas com dados faltantes, como o valor total e com registros foram do padrão observado nas demais colunas, possivelmente causado por questões de registro no banco de dados. 
Após essa limpeza foi possível visualizar os dados por meio de gráfico de linhas para compreensão sobre a tendência dos custos no sistema de saúde dividido por unidade federativa. A participaçao dos custos por unidade federativa foi melhor visualizada por meio do gráfico de barras. 
Aqui foi aplicado recursos do matplotlib para melhorar a visualização do gráfico, bem como seleção de unidades federativas específicas para visualização.

### Manipulação de dados
Na manipulação foi aplicado uma palete de cores para melhorar a visualização do gráfico de linhas, mas sem muito sucesso dado a quantidade de informação disposta no gráfico. Foi adicionado mais uma coluna referente a região na qual a unidade federativa pertence, mas não foi possível realizar análise com a inclusão dessa coluna diretamente ao dados.
Foi observado dados refente a notificações de dengue para corelação aos custos do DATASUS, mas não foi possível tirar conclusões com os dados dos últimos meses. Também foram feitas comparações dos dodos com o estado da Bahia (meu estado).

### Análise de gráficos e criação de hipóteses
Foi observado como a configuração e apresentação do gráfico pode influenciar na interpretação visual e tendencionamento das conclusões.

### Manipulação e interpretação de gráficos
Para ampliar a visão sobre os custos foi agregado a informação referente a população por estado, por meio da biblioteca urllib.reques e BeautifulSoup foi possível coletar as informações do site do Wikipédia (https://pt.wikipedia.org/wiki/Lista_de_unidades_federativas_do_Brasil_por_popula%C3%A7%C3%A3o), as informações dispostas no site estão muito próximas ao site do IBGE (https://www.ibge.gov.br/apps/populacao/projecao/).
Foi possível observar a relação de custos e tamanho da população.
Por meio dos dados referente ao custo médio por internação foi visto que a região sul do país possuem as maiores médias. 
