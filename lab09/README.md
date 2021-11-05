# Lab09 - Grafo de Conhecimento

# Aluno
* 256352: Cristiano Sampaio Pinheiro

## Exemplo de Grafo de Conhecimento - para publicar ou enriquecer
Partindo do tema escolhido, filmes, percebemos que as bases de dados adotadas inicialmente apresentam alguns dados faltantes, como classificação indicativa por exemplo, para certos títulos. Partindo disso, com as ferramentas apresentadas em sala é possível montar uma rotina que busca por esses títulos na dbpedia e extrai os dados faltantes.  
Indo além de completar os dados faltantes, ainda usando a dbpedia é possível captar mais informações sobre as pessoas que participaram das obras. Podemos complementar as informações de atores e diretores com dados como: idade, nacionalidade, quanto tempo atua no mercado cinematográfico e prêmios.  
Por fim, há alguns dados a se acrescentar nas mídias, como a empresa resposável pela distribuição. Para as séries é possível acrescentar a informação do número total de episódios e para os filmes também podemos acrescentar a arrecadação obtida com aquele título.  
Com essas adições o esquema do banco de dados ficaria como na Figura 1.

![Esquema do banco de dados](/images/esquemaDB.png)
_Figura 1: Esquema do banco de dados_

## Perguntas de Pesquisa ou Queries

* Pergunta 1  
  Partindo das informações adicionadas para diretores e atores, podemos analisar se a idade influência no gênero que essas pessoas atuam. Mais do que isso, podemos verificar se pessoas que trabalham no meio a mais tempo tendem a participar de obras mais bem avaliadas e populares, ou mesmo se são as que mais acumulam prêmios.
* Pergunta 2  
  Acrescentando a informação da organização responsável pela distribuição da mídia, podemos analisar quais dessas empresas facilitam a distribuição a partir de uma comparação da data de lançamento com a data de disponibilização nos serviços de streaming. Com base nesses dados pode ser possível predizer em quanto tempo um certo título distibuído por uma companhia levará para ser disponibilizado nos serviços de streaming com base na sua data de lançamento.
* Pergunta 3  
  Partindo da ideia apresentada na pergunta anterior e unindo a informação da arrecadação adicionada para os filmes, podemos verificar se mídias que são amplamente distribuídas pelas plataformas de streaming arecadam mais, ou ainda, se materiais exclusivos são mais lucrativos. Por fim, é possível verificar se participantes(atores/diretores) populares garantem uma arrecadação maior.
