# Introdução à Programação e Ferramentas Computacionais para as Ciências Sociais

- Responsável: Leonardo S. Barone
- Adaptado por: Nathan Giachetta
- Data: definir

## Desafio 1

## Instruções para Entrega

Data: definir

Formato: RScript (arquivo .R)

Via: e-mail com título "[R-CiênciasSociais] - D1".

## Instruções para a atividade

Siga as instruções abaixo. Documente __TODOS__ os seus passos em um script. Comente no seu script __TODOS__ os seus passos e explique a si mesm@ suas escolhas e estratégias. Colar pedaços de código nesta atividade é permitido e peça ajuda se precisar. Mencione __SEMPRE__ em comentários quando a solução encontrada não for sua.

As primeiras linhas do seu script devem conter suas informações pessoais como comentário, tal qual o modelo abaixo:

```{r}
### nome <- "Fulano da Silva Sauro"
### graducao <- "Primeiro ano"
### n_usp <- 32165498
### data_entrega: ""
```

### Parte 1 - abrindo os dados

1- Vá ao [Repositório de Dados Eleitorais do TSE](http://www.tse.jus.br/eleitor-e-eleicoes/estatisticas/repositorio-de-dados-eleitorais-1/repositorio-de-dados-eleitorais). Faça o download do arquivo de resultados de 2016 e descompacte-o. Você pode fazer tudo à mão se tiver dificuldade de copiar o modelo do [tutorial 4](https://github.com/ngiachetta/FLS6397/blob/master/tutorials/tutorial4.Rmd), em que abrimos os dados da MUNIC 2005. (Nome do arquivo: "Votação __nominal__ por município e zona")

2- Importe para o R os dados de Votação nominal de 2016.

3- Crie um _data frames_ denominado  _candidatos_, com informações sobre as as votações nominais dos 3 estados do sul, respectivamente.

(Dica: use a função _rbind_ ou a função _bind\_rows_, que é o equivalente melhorado do dplyr, para juntar os _data frames_ )

### Parte 2 - _data frame_ resultados

4- Selecione apenas as linhas que contém CANDIDATOS para prefeit@ e guarde no mesmo dataframe chamado _candidatos_.

5- Mantenha no banco de dados apenas as linhas que contém informações sobre UF, UE, sigla do partido, número do partido e nome do candidat@ com os seguintes nomes, respectivamente: uf, ue, partido, num_cand, nome.

Se você tiver dúvida sobre as colunas e nomes das variáveis, consulte o arquivo "LEIAME.pdf" que vem em conjunto com os dados do repositório.

(Dicas: use as funções _filter_, _rename_ e _select_ do pacote dplyr)

### Parte 3 - agregando e combinando por candidato

6 - Usando as funções _group\_by_ e _sumarise_, produza um novo _data frame_ que apresente a presença dos partidos na eleição. Chame esse novo _data frame_ de _partidos\_cand_. Dica: para contar os partidos use a função `n()` sem nenhum argumento.

### Bônus
7 - O que acontece se utilizamos a função _count()_ do dplyr para o mesmo objetivo do exercício anterior?
