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

### Parágrafos e quebras de linha

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

### Simbolos

Para que algum símbolo apareça no conteúdo do site, não basta simplesmente colocá-lo no código. Então é necessário usar 
caracteres especiais que se referem ao código desses símbolos. [Link](https://dev.w3.org/html5/html-author/charref) para consultar o código de cada símbolo. 

O mesmo pode ser feito com emojis, usando o parâmetro **&#x** seguido do código hexadecimal do emoji. Para consulta dos códigos o [link é esse](https://emojipedia.org).

### Imagens

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

### Hierarquia de Títulos

Títulos em HTML são chamados headings, onde possuem 6 níveis que são expecificados pelas tags: < h1 >, < h2 >, < h3 >, < h4 >, < h5 > e < h6 >. 
< h1 > Se refere ao título principal, enquanto aos outros são subníveis de < h1 >. 

### Formatações

* Negrito: recomendado o uso de < strong >;
* Itálico: < em >;
* Marca texto: < mark >...< /mark >;
* Texto pequeno: < small >;
* Texto deletado: < del >;
* Texto inserido: < ins >...< /ins >;
* Texto sobrescrito: < sub >;
* Texto subscrito: < sup >;
* Trecho de código: < code >...< /code > & < pre > (mantém a pré-formatação);
* Citações: < q >;
* Citações em blocos: < blockquote >;
* Abreviações: < abbr >;

### Listas

* Listas ordenadas: criada e delimitada pela tag < ol > e onde cada ítem é listado pela tag < li >. Existem os parâmetros *type* 
(para configurar o tipo de marcador da lista) e também o *start* (para configurar o início da contagem).
* Listas não ordenadas: criada e delimitada pela tag < ul >, onde cada ítem também é listado pela tag < li >. O parâmetro *type* 
pode modificar o tipo do marcador, podendo ser **disc, circle** ou **square**, sendo o *disc* o padrão. 

Obs: as listas podem feitas umas dentro das outras, ou seja, podem ser mistas. 

* Lista de definição: termo principal marcado pela tag < dt > e sua explicação < dd >;

### Links e Âncoras

* Links: tag < a >...< /a > onde o parâmetro *href* deve ser preenchido com a URL de caminho. Além disso pode-se utilizar o parâmetro 
*hreflang* para indicar o idioma principal do site que está sendo linkado. É recomendável o uso do atributo *target* para os 
seguintes valores: 
 * _blank: abrir o link em uma nova janela em branco;
 * _self: abrir o link na janela ou frame atual (padrão);
 * _top: desfaz todos os frames e abre o destino no navegador completo;
 * _parent: similar ao _top em uma referência à janela mãe nome-do-frame caso esteja usando frames, indicar o nome da janela a abrir.
O atributo *rel* é utilizado para indicar a natureza do destino:
 * next: indica que o link é para a próxima parte do documento atual;
 * prev: '' para anterior do documento atual;
 * author: '' para o site do autor do artigo atual;
 * external: '' para o site que não faz parte do site. 
Para fazer downloads é utilizado a mesma tag < a > e o parâmetro *href*, com o complemento de parâmetros *download* (e indicar o nome do arquivo) e 
*type* ([tipo de arquivo](https://www.iana.org/assignments/media-types/media-types.xhtml)).

### Mídias

* Imagens dinâmicas: para casos de adaptação, seja ao diminuir a janela do navegador ou ao abrir o site em outros dispositivos. Para isso 
usa-se a tag < picture > e < source >. A tag < img > irá ser utilizada normalmente, porém acima dela a *source* é usada para que o carregamento 
das outras imagens sejam feitas de acordo com o tamanho necessário (da menor para a maior). A tag *source* possui três parâmetros: media (tamanho 
máximo a ser considerado para a imagem ser carregada), srcset (nome do arquivo da imagem) e type (indicando o tipo de imagem).
* Audios: utiliza-se a tag < audio > (com parâmetros como controls, autoplay, loop, preload="metadata") em conjunto com a tag < source src > 
(que indicará o nome do arquivo e seu tipo).
* Vídeos: usa-se a tag < video > (com parâmetros como: width, poster, controls, autoplay, etc.) para vídeos hospedados no próprio servidor. 
Novamente a tag *source scr* é usada para indicar o nome do arquivo e seu tipo. Para vídeos hospedados em outros sites, como o youtube 
por exemplo, existe a função **incorporar**, assim aparece-rá um script personalizado para ser copiado e colado em seu arquivo. 

# CSS

## Estilos

### Estilo inline

São estilos colocados linha a linha do seu código. Ex: 

```
<body style="font-family: Arial;">
```

Dessa forma, a fonte de todo o conteúdo de seu site estará com a fonte Arial. O problema desse estilo é a poluição no código, pois 
se quiser mudar, por exemplo, a fonte apenas dos títulos de hierarquia 1, o estilo terá que ser feito em cada um dos títulos, ocupando 
espaço e tempo. **Porém para casos mais específicos, que sejam necessárias configurações pontuais, esse estilo é mais recomendado**.

### Estilo interno

Esse tipo de estilo é feito com base em seletores atraves da tag < style > abaixo da tag *title*. Os seletores seguem a seguinte 
configuração:

```
<style>
    body {
        font-family: Arial, Helvetica, sans-serif;
    }

    h1 {
        color: greeen;
    }
</style>
```

Assim, nesse exemplo, todos os títulos de hierarquia 1 possuem a cor verde. Esse estilo é mais limpo e deixa claro a separação entre 
*conteúdo* e *forma*. O problema encontra-se quando o site possuí várias páginas com o mesmo estilo, pois esse código deverá ser copiado 
em todas, assim criando códigos extensos. 

### Estilos externos

Dentro da tag < head > usa-se a tag *link css*, referenciando assim um arquivo **.css** separado. O código é construído de forma semelhante 
à maneira interna. 

```
@charset "UTF-8"; /* regra caso haja problemas com acentuação */

body {
        font-family: Arial, Helvetica, sans-serif;
    }

    h1 {
        color: greeen;
    }
```

O resultado será o mesmo do estilo interno, porém agora em um arquivo separado que pode ser linkado em todas as páginas. 