<!DOCTYPE html>
<html>

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AluraBooks</title>
    <link rel="stylesheet" href="reset.css">
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1>Alurabook</h1>
</body>
</html>
‎reset.css
+135
Original file line number	Diff line number	Diff line change
@@ -0,0 +1,135 @@
/* http://meyerweb.com/eric/tools/css/reset/ 
   v2.0 | 20110126
   License: none (public domain)
*/
html,
body,
div,
span,
applet,
object,
iframe,
h1,
h2,
h3,
h4,
h5,
h6,
p,
blockquote,
pre,
a,
abbr,
acronym,
address,
big,
cite,
code,
del,
dfn,
em,
img,
ins,
kbd,
q,
s,
samp,
small,
strike,
strong,
sub,
sup,
tt,
var,
b,
u,
i,
center,
dl,
dt,
dd,
ol,
ul,
li,
fieldset,
form,
label,
legend,
table,
caption,
tbody,
tfoot,
thead,
tr,
th,
td,
article,
aside,
canvas,
details,
embed,
figure,
figcaption,
footer,
header,
hgroup,
menu,
nav,
output,
ruby,
section,
summary,
time,
mark,
audio,
video {
    margin: 0;
    padding: 0;
    border: 0;
    font-size: 100%;
    font: inherit;
    vertical-align: baseline;
}
/* HTML5 display-role reset for older browsers */
article,
aside,
details,
figcaption,
figure,
footer,
header,
hgroup,
menu,
nav,
section {
    display: block;
}
body {
    line-height: 1;
}
ol,
ul {
    list-style: none;
}
blockquote,
q {
    quotes: none;
}
blockquote:before,
blockquote:after,
q:before,
q:after {
    content: '';
    content: none;
}
table {
    border-collapse: collapse;
    border-spacing: 0;
}
‎styles.css
+11
Original file line number	Diff line number	Diff line change
@@ -0,0 +1,11 @@
:root {
    --cor-de-fundo: #EBECEE;
}
body {
    background-color: var(--cor-de-fundo);
}
h1 {
    background-color: white;
}display: block;
        top: 60%;
    }
    .card {
        width: 40%;
        margin: 2em auto;
    }
}

@media screen and (min-width: 1728px) {
    .carrossel__container {
        display: flex;
        margin: 0 20vw 3em 20vw;
        align-items: center;
    }

    .swiper-pagination {
@@ -121,10 +115,6 @@
        font-size: 16px;
    }

    .descrição {
        margin-right: 2em;
    }
    .card {
        width: 60%;
        margin-left: 3em;
@@ -101,7 +101,7 @@ <h2 class="carrossel__titulo">Novos lançamentos</h2>
        <!-- Additional required wrapper -->
        <div class="swiper-wrapper">
          <!-- Slides -->
          <div class="swiper-slide"><img src="img/Apachekafka.svg"
          <div class="swiper-slide"><img src="img/ApacheKafka.svg"
              alt="Livro sobre apache kafka e spring boot da alura books"></div>
          <div class="swiper-slide"><img src="img/Liderança.svg"
              alt="Livro sobre liderança em design design da alura books"></div>
@@ -245,7 +245,7 @@ <h2 class="contato__titulo">Fique por dentro das novidades!</h2>
        Atualizações de e-books, novos livros, promoções e outros.
      </p>
    </div>
    <input type="email" placeholder="         Cadastre seu e-mail" class="contato__email" />
    <input type="email" placeholder="        Cadastre seu e-mail" class="contato__email">
  </section>

  <hr />
@@ -335,8 +335,8 @@ <h2 class="rodapé__titulo">Grupo Alura</h2>
      spaceBetween: 10,
      slidesPerView: 3,
      pagination: {
        el: ".swiper-pagination",
        type: "bullets",
        el: '.swiper-pagination',
        type: 'bullets',
      },
    });
  </script>
‎styles/contato.css
+2
-4
Original file line number	Diff line number	Diff line change
@@ -32,11 +32,10 @@
.contato__email::placeholder {
    font-family: var(--fonte-principal);
    color: var(--azul);
    background: url("../img/email.svg") no-repeat 5%;
    padding-left: 5em;
    background: url("../img/Email.svg") no-repeat 5%;
    padding-left: 2em;
}

@media screen and (min-width: 1024px) {
    .contato {
        display: flex;
@@ -58,7 +57,6 @@
    }
}

@media screen and (min-width: 1728px) {
    .contato {
        padding: 3em 20vw;@@ -240,6 +240,81 @@ <h2 class="contato__titulo">Fique por dentro das novidades!</h2>

  <footer class="rodapé">
    <h2 class="rodapé__titulo">Grupo Alura</h2>
    <ul class="lista-rodapé">
      <li class="lista-rodapé__titulo">Educação</li>
      <li class="lista-rodapé__item">
        <img src="img/Caelum.svg" alt="Logo da Caelum" />
        <a href="#" class="lista-rodapé__link">Caelum</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/CasaDoCodigo.svg" alt="Logo da Casa do Código" />
        <a href="#" class="lista-rodapé__link">Casa do Código</a>
      </li>
    </ul>
    <ul class="lista-rodapé">
      <li class="lista-rodapé__titulo">Educação online</li>
      <li class="lista-rodapé__item">
        <img src="img/Alura.svg" alt="Logo da Alura" />
        <a href="#" class="lista-rodapé__link">Alura</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/AluraEmpresas.svg" alt="Logo da AluraParaEmpresas" />
        <a href="#" class="lista-rodapé__link">Alura para Empresas</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/AluraLATAM.svg" alt="Logo da Alura Latam" />
        <a href="#" class="lista-rodapé__link">Alura LATAM</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/AluraStart.svg" alt="Logo da Alura START" />
        <a href="#" class="lista-rodapé__link">Alura Start</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/MusicDot.svg" alt="Logo da Music Dot" />
        <a href="#" class="lista-rodapé__link">Music Dot</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/AluraLingua.svg" alt="Logo da Alura Lingua" />
        <a href="#" class="lista-rodapé__link">Alura Língua</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/PM3.svg" alt="Logo da PM3" />
        <a href="#" class="lista-rodapé__link">PM3</a>
      </li>
    </ul>
    <ul class="lista-rodapé">
      <li class="lista-rodapé__titulo">Comunidade</li>
      <li class="lista-rodapé__item">
        <img src="img/HipstersTech.svg" alt="Logo do Hipsters ponto Tech" />
        <a href="#" class="lista-rodapé__link">Hipsters ponto Tech</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/ScubaDev.svg" alt="Logo do Scuba Dev" />
        <a href="#" class="lista-rodapé__link">Scuba Dev</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/LayersTech.svg" alt="Logo do Layers ponto Tech" />
        <a href="#" class="lista-rodapé__link">Layers ponto Tech</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/LikeABoss.svg" alt="Logo do Like a Boss" />
        <a href="#" class="lista-rodapé__link">Like a Boss</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/CarreiraSemFronteira.svg" alt="Logo do Carreira sem fronteiras" />
        <a href="#" class="lista-rodapé__link">Carreira sem fronteiras</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/HipstersJobs.svg" alt="Logo do Hipsters ponto jobs" />
        <a href="#" class="lista-rodapé__link">Hipsters ponto jobs</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/GUJ.svg" alt="Logo do GUJ" />
        <a href="#" class="lista-rodapé__link">GUJ</a>
      </li>
    </ul>
  </footer>

  <script src="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.js"></script>
‎styles.css
+2
Original file line number	Diff line number	Diff line change
@@ -15,6 +15,8 @@
    --azul: #002F52;
    --fonte-secundario: "Josefin Sans";
    --preto: #000000;
    --cinza: #474646;
    --cinza-claro: #858585;
}

body {
‎styles/rodapé.css
+37
Original file line number	Diff line number	Diff line change
@@ -5,4 +5,41 @@ hr {
.rodapé {
    background-color: var(--branco);
    padding: 1em;
}
.lista-rodapé {
    display: none;
}
@media screen and (min-width: 1024px) {
    .rodapé {
        display: flex;
        justify-content: space-around;
    }
    .lista-rodapé {
        display: block;
    }
    .lista-rodapé__item {
        display: flex;
        align-items: center;
        margin: 0.6em 0;
    }
    .lista-rodapé__link {
        color: var(--cinza);
        text-decoration: none;
        margin-left: 0.6em;
    }
    .lista-rodapé__titulo {
        font-size: 14px;
        color: var(--cinza-claro);
    }
    .rodapé__titulo {
        font-size: 24px;
    }
}
