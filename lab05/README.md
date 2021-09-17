# Lab05 - Marcadores e Taxonomia em Cypher

# Aluno
* 256352: Cristiano Sampaio Pinheiro

## Tarefa de Cypher sobre Marcadores e Taxonomia

## Tarefa 1

Escreva em Cypher uma consulta que retorne os marcadores da categoria `Serviços`, sem considerar as categorias subordinadas.

### Resolução
~~~cypher
MATCH  (m:Marcador)-[:Pertence]->(c:Categoria {id:"Serviços"})
RETURN m
~~~

## Tarefa 2

Escreva em Cypher uma consulta que retorne os marcadores da categoria `Serviços`, considerando as categorias subordinadas.

### Resolução
~~~cypher
MATCH  (m:Marcador)-[:Pertence]->(c1:Categoria)-[*]->(c2:Categoria {id:"Serviços"})<-[:Pertence]-(m1:Marcador)
RETURN m, m1
~~~
