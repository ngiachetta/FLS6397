# Introdução à Programação e Ferramentas Computacionais para as Ciências Sociais

- Responsável: Leonardo S. Barone
- Adaptado por: Nathan Giachetta
- Data: definir

## Desafio 5

## Instruções para Entrega

Data: definir

Formato: 2 arquivos: (1) RScript (arquivo .R); (2) arquivo .pdf ou .html produzido com RMarkdown.

Via: e-mail com título "[R-CiênciasSociais] - D5".

__OBS: VOCÊ PODE FAZER ESTA ATIVIDADE SOZINH@ OU EM GRUPO DE ATÉ 3 PESSOAS__

## Instruções para a atividade

Siga as instruções abaixo. Faça no arquivo de RMarkdown uma síntese de sua atividade e apresente apenas o essencial do código (você deve julgar o que é essencial).

Documente __TODOS__ os seus passos no arquivo de script. Comente no seu script __TODOS__ os seus passos e explique a si mesm@ suas escolhas e estratégias.

O arquivo .pdf ou .html produzido em RMarkdown deve contar as informações dos integrantes do grupo.

As primeiras linhas do seu script devem conter suas informações pessoais como comentário, tal qual o modelo abaixo:

```{r}
### nome <- c("Fulano da Silva Sauro","Fulana da Silva Sauro","Sauro da Silva Fulano")
### graducao <- c("Primeiro ano", "Segundo ano", "Quarto ano")
### n_usp <- c(32165438,78165598, 43895498)
### data_entrega: ""
```

### Parte 1 - Coletando um "corpus" com webscrapping

Coleta um conjunto de textos com webscrapping. Você pode coletar notícias de jornal, registros administrativos ou textos de qualquer natureza, desde que contenham um número relevantes de caracteres cada (pelo menos 2 parágrafos) e sejam "discursivos", ou seja, não contenham exclusivamente informações técnicas.

Se você pretende usar o pacote _rvest_ e precisa de exemplos, veja a documentação da aula 8. Postei lá os exemplos que fizemos em sala de aula.

### Parte 2 - Pré-processamento + nuvem de palavras

Utilizando o pacote _tm_, crie um objeto da classe "Corpus" e faça o pré-processamento do texto. Construa uma nuvem de palavras com o resultado.

### Parte 3 - Pré-processamento + nuvem de palavras

Utilizando o pacote _tidytext_, construa um gráfico de barras dos temos mais frequêntes. Repita o mesmo procedimento para "bigrams".

### Fim
