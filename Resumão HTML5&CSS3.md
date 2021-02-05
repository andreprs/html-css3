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
# HTML

## Parágrafos e quebras de linha

Os parágrafos em HTML são **delimitados pelas tags < p > e </ p >**, porém isso mantém o texto todo junto, mesmo havendo 
quebra de linha a linguagem não interpretará dessa forma. EX: 

```
<p> Esse é um 
    parágrafo
    feito em 
    HTML.
</p>
```

O resultado será:

```
Esse é um parágrafo feito em HTML.
```

Para que haja a quebra de linha **pode-se usar a tag < br >**, que significa "break row" (quebre a linha). 

## Simbolos

Para que algum símbolo apareça no conteúdo do site, não basta simplesmente colocá-lo no código. Então é necessário usar 
caracteres especiais que se referem ao código desses símbolos. [Link](https://dev.w3.org/html5/html-author/charref) para consultar o código de cada símbolo. 

O mesmo pode ser feito com emojis, usando o parâmetro **&#x** seguido do código hexadecimal do emoji. Para consulta dos códigos o [link é esse](https://emojipedia.org).

## Imagens

* Sites com imagens de domínio público: [Unsplash](https://unsplash.com), [Pexels](https://www.pexels.com/pt-br/), [Rawpixel](https://www.rawpixel.com/?sort=shuffle&page=1&feed=creative-feed), [Pixabay](https://pixabay.com/pt/), [Flaticon](https://www.flaticon.com/br/), etc.

Os formatos de imagens mais utilizados na criação de sites são o **JPEG** e **PNG** (possui transparência), pois possuem certa compactação, deixando assim a imagem mais leve. 

É preferível que a resolução da imagem a ser utilizada seja pequeno (de acordo com a necessiodade), para que isso não torne o site lento. Para 
redimensionar uma imagem pode-se utilizar qualquer programa de manipulação de imagem, como o GIMP ou o Photoshop.

Existem três maneiras básicas de se carregar uma imagem no código HTML. Duas delas envolvem os arquivos do próprio computador que estejam 
na mesma pasta do arquivo **index.html** (sub-pastas também contam) ou utilizando o link da imagem. Digitando **img** 
o editor já completa a linha de código, bastando completar com o arquivo de imagem. 
Quando a imagem está na mesma pasta do arquivo **index** pode-se utilizar o atalho **ctrl+espaço** do editor *VScode* e selecionar o arquivo que deseja utilizar.

### Favicon

Em um site é possível adicionar um ícone de favicon digitando *link:favicon* no VScode. **É recomendável o uso de arquivos com a extensão** *.ico*. 

Sites recomendados: 

* Site para criar seu próprio ícone: [favicon.cc](https://www.favicon.cc)
* Site para conversão de outros formatos para ícone: [favicon.io](https://www.favicon.cc)
