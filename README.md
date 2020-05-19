# primeros passos com leaflet

## breve introdução a web

paginas web são compostas em sua maioria por arquivos estaticos com funções especificas. Um arquivo HTML que contem os elementos da pagina, um arquivo CSS que adiciona estilo nos elementos da pagina como tamanho da fonte, cor, layout etc.. E um arquivo JavaScript que contem a logica da pagina.

Para saber, é possível manter um unico arquivo html e deixar o css e javascript contidos nesse arquivo, porem isso não é recomendado de acordo com as boas praticas.

--------

## alguns recursos para aprender:

[minicurso de html](https://www.youtube.com/watch?v=UB1O30fR-EE&t=324s)


[minicurso de css](https://www.youtube.com/watch?v=yfoY53QXEnI&list=PLillGF-RfqbZTASqIqdvm1R5mLrQq79CU&index=2)


[minicurso de javascript](https://www.youtube.com/watch?v=hdI2bqOjy3c)

-------------

## bibliotecas javascript 

antes de explicar o leaflet em si, é preciso entender oque são bibliotecas de código. Como já foi dito, as boas praticas nos dizem que o correto é manter a logica separada do elementos da pagina e do estilo, para isso criamos um arquivo javascript idependente e é nele que construimos o código da pagina. 

suponha que tenhamos um arquivo chamado `app.js` como nosso código, para usar esse código devemos chamar o arquivo js dentro do arquivo html, para fazer isso usamos a seguinte html 
    
    <script src="app.js"></script>

lembre-se de colocar essa tag no final do arquivo e de se certificar de que o arquivo js está na mesma pasta que o arquivo html.

----------

bibliotecas javascript nada mais são do que arquivos js que possuem códigos especificos para alguma funcionalidades que estão "hosteados" na nuvem, dessa maneira não é preciso ter o arquivo na sua maquina para poder usar o código, apenas referenciar a biblioteca como fizemos com o arquivo `app.js`

----------

## leaflet

é comum que as bibliotecas disponibilizem URLs para fazer o importe da biblioteca em projetos alheios. No caso do leaflet, a versão da linguagem disponibiliza as seguintes url

javascript

    <link rel="stylesheet" href="https://unpkg.com/leaflet@1.6.0/dist/leaflet.css"
        integrity="sha512-xwE/Az9zrjBIphAcBb3F6JVqxf46+CDLwfLMHloNu6KEQCAWi6HcDUbeOfBIptF7tcCzusKFjFw2yuvEpDL9wQ=="
        crossorigin="" />

css

    <script src="https://unpkg.com/leaflet@1.6.0/dist/leaflet.js"
        integrity="sha512-gZwIG9x3wUXg2hdXF6+rVkLF/0Vi9U8D2Ntg4Ga5I5BZpVkVxlJWbSQtXPSiUTtC0TjtGOmxa1AJPuV0CPthew=="
        crossorigin=""></script>

coloque esses dois snippets no head do seu arquivo html

-----