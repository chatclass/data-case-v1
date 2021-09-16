# Case chatclass

## Introdução

Olá! Se você está vendo esta mensagem, deve ser um candidado para nosso time de dados!
Este case serve para identificar em você as principais habilidades técnicas que estão em nosso dia a dia aqui na ChatClass. 
Sendo assim, lhe desejamos boa sorte e vamos ao que interessa :)

## Como vai funcionar?

Gosta de filmes? Então você vai amar esse desafio! Neste case você irá trabalhar com dados retirados do site [Kaggle](https://www.kaggle.com/tmdb/tmdb-movie-metadata). 

O objetivo é testar 3 habilidades:

1. ETL com python
2. SQL
3. Uso de API's REST

Para isso, vamos precisar que execute as seguintes tarefas:

### ETL com Python:

Na tabela credits, extraia da coluna **crew** (lista de pessoas) quem é o diretor do filme (nome e ID). Pra isso, basta encontrar na lista de pessoas, alguém cujo **job** é **Director** (cuidado com case sensitive). Alguns filmes não vão ter essa informação, mas são bem poucos.

### SQL

Após conseguir adicionar o nome do diretor e seu ID em cada linha da tabela credits, crie um banco de dados SQLite e insira as duas tabelas (movies e credits) no banco, utlizando formatos coerentes para as colunas. Não é necessário inserir as colunas JSON, pode descartá-las.

Agora, através de queries SQL, consiga o **budget** total (somatório) de todos os filmes para cada um dos diretores. Os diretores estão na tabela credits e os budgets na tabela movies.

### API REST

Depois de ver um bom filme bate aquele tédio, não é? Bom, a atividade desta etapa é consultar (via python) esta [API](https://www.boredapi.com/documentation) através de um GET e buscar uma atividade para matar o tédio!