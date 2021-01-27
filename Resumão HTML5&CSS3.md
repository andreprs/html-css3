# Conceitos Básicos

* DNS (Domain Name System): espécie de "lista telefônica" que criam ligações entre o nome do site que se deseja acessar 
e o número de IP relacionado a ele. 

* Domínio: nome único que identifica o servidor ou página. Os domínios apresentam um TLD (Top Level Domain), que podem 
ser GTLD (TLD's genéricos) ou ccTDL (country code).

* Hospedagem: serviço que hospeda os arquivos para que o site continue disponível, seguro e mantenha sua performance. 

# HTML5 e CSS3

* HTML: o significado da sigla é "Hypertext Markup Language", ou seja, uma linguagem de marcação hipertexto. A HTML é 
**responsável pelo conteúdo da página**.

* CSS: o significado da sigla é "Cascading Style Sheets", ou seja, folhas de estilo em cascata. As CSS's são 
**responsáveis pelo estilo da página**, como a fonte, seu tamanho, cor, entre outros. 

## Tags HTML

A HTML funciona com marcações específicas chamadas **tags**, que são um conjunto de palavras entre sinais de **colchete angular**. EX: 

```
<p>Exemplo de parágrafo</p>
```
* Onde a primeira tag representa a sua abertura, a última seu fechamento e o que se encontra dentro das *tags* é o conteúdo. 

## Seletores CSS

```
p {
    font-family: Arial;
    font-size: 12pt;
    color: blue;
}
```

* Onde: 
  * A linha toda trata-se da declaração;
  * A especificação antes do dois pontos trata-se da propriedade;
  * A especificação depois dos dois pontos trata-se do valor;
  * *p* antes dos colchetes trata-se do seletor.

## Estruta básica de um documento HTML

```
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
<head>
<body>

<body>
</html>
```
