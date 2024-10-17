‎img/ScubaDev.svg
+9



‎img/Usuario.png
Binary file not shown.
‎img/Usuario.svg
+3



‎img/Usuário.svg
-3
This file was deleted.
‎img/menu_black_24dp 1.png
Binary file not shown.‎img/ScubaDev.svg
+9



‎img/Usuario.png
Binary file not shown.
‎img/Usuario.svg
+3



‎img/Usuário.svg
-3
This file was deleted.
‎img/menu_black_24dp 1.png
Binary file not shown.
Original file line number	Diff line number	Diff line change
@@ -11,27 +11,27 @@
    background-clip: text;
}

.contato__titulo {
    font-size: 18px;
    font-weight: 500;
}

.contato__texto {
    font-weight: 300;
    margin: 1em 0;
}

.contato__email {
    padding: 1em;
    border: 1px solid var(--azul);
    border-radius: 24px;
    width: 90%;
    color: var(--azul);
}

.contato__email::placeholder {
    font-family: var(--fonte-principal);
    color: var(--azul);
    background: url("../img/Email.svg") no-repeat;
    background: url("../img/Email.svg") no-repeat 5%;
    padding-left: 2em;
}Original file line number	Diff line number	Diff line change
@@ -1 +1,17 @@
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
}Original file line number	Diff line number	Diff line change
@@ -193,6 +193,20 @@ <h2 class="tópicos__titulo">TÓPICOS VISITADOS RECENTEMENTE</h2>
    </ul>
  </section>

  <section class="contato">
    <h2 class="contato__titulo">Fique por dentro das novidades!</h2>
    <p class="contato__texto">
      Atualizações de e-books, novos livros, promoções e outros.
    </p>
    <input type="email" placeholder="Cadastre seu e-mail" class="contato__email" />
  </section>
  <hr />
  <footer class="rodapé">
    <h2 class="rodapé__titulo">Grupo Alura</h2>
  </footer>
  <script src="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.js"></script>
  <script>
    const swiper = new Swiper(".swiper", {
‎styles.css
+2
Original file line number	Diff line number	Diff line change
@@ -2,6 +2,8 @@
@import url("styles/banner.css");
@import url("styles/carrossel.css");
@import url("styles/topicos.css");
@import url("styles/contato.css");
@import url("styles/rodapé.css");

:root {
    --cor-de-fundo: #EBECEE;
‎styles/contato.css
+37
Original file line number	Diff line number	Diff line change
@@ -0,0 +1,37 @@
.contato {
    background-color: var(--branco);
    padding: 1em;
}
.contato__titulo,
.contato__texto {
    background: var(--azul-degrade);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
}
.contato__titulo {
    font-size: 18px;
    font-weight: 500;
}
.contato__texto {
    font-weight: 300;
    margin: 1em 0;
}
.contato__email {
    padding: 1em;
    border: 1px solid var(--azul);
    border-radius: 24px;
    width: 90%;
    color: var(--azul);
}
.contato__email::placeholder {
    font-family: var(--fonte-principal);
    color: var(--azul);
    background: url("../img/Email.svg") no-repeat;
    padding-left: 2em;
}
‎styles/rodapé.css
+8
Original file line number	Diff line number	Diff line change
@@ -0,0 +1,8 @@
hr {
    margin: 0;
}
.rodapé {
    background-color: var(--branco);
    padding: 1em;
}  <section class="contato">
    <h2 class="contato__titulo">Fique por dentro das novidades!</h2>
    <p class="contato__texto">
      Atualizações de e-books, novos livros, promoções e outros.
    </p>
    <input type="email" placeholder="Cadastre seu e-mail" class="contato__email" />
  </section>
  <hr />
  <footer class="rodapé">
    <h2 class="rodapé__titulo">Grupo Alura</h2>
  </footer>
  <script src="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.js"></script>
  <script>
    const swiper = new Swiper(".swiper", {
‎styles.css
+2
Original file line number	Diff line number	Diff line change
@@ -2,6 +2,8 @@
@import url("styles/banner.css");
@import url("styles/carrossel.css");
@import url("styles/topicos.css");
@import url("styles/contato.css");
@import url("styles/rodapé.css");

:root {
    --cor-de-fundo: #EBECEE;
‎styles/contato.css
+37
Original file line number	Diff line number	Diff line change
@@ -0,0 +1,37 @@
.contato {
    background-color: var(--branco);
    padding: 1em;
}
.contato__titulo,
.contato__texto {
    background: var(--azul-degrade);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
}
.contato__titulo {
    font-size: 18px;
    font-weight: 500;
}
.contato__texto {
    font-weight: 300;
    margin: 1em 0;
}
.contato__email {
    padding: 1em;
    border: 1px solid var(--azul);
    border-radius: 24px;
    width: 90%;
    color: var(--azul);
}
.contato__email::placeholder {
    font-family: var(--fonte-principal);
    color: var(--azul);
    background: url("../img/Email.svg") no-repeat;
    padding-left: 2em;
}
‎styles/rodapé.css
+8
Original file line number	Diff line number	Diff line change
@@ -0,0 +1,8 @@
hr {
    margin: 0;
}
.rodapé {
    background-color: var(--branco);
    padding: 1em;
}
