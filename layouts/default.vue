<template lang="pug">
div
  BaseHeader
  nuxt.container
  BaseFooter
</template>

<style>
body {
  background: skyblue;
}
* {
  break-before: auto;
  break-after: auto;
  break-inside: avoid-column;
  -moz-break-before: auto;
  -moz-break-after: auto;
  -moz-break-inside: avoid-column;
  -webkit-break-before: auto;
  -webkit-break-after: auto;
  -webkit-break-inside: avoid-column;
}

/*entete
		background: teal;
*/
header {
  height: 150px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  text-align: center;
  margin: 0.2em 0.4em;
  border-radius: 10px;
}

h1,
h2,
h3 {
  color: black;
  text-shadow: 0px 0px 3px white, 0 0 5px grey;
}

h2 {
  font-style: italic;
}
h3 {
  text-decoration: underline;
}

.home {
  list-style-type: none;
  padding: 0.2em 0.4em;
  border-radius: 10px;
  border: medium black ridge;
  width: 6em;
}

.home a {
  text-decoration: none;
}

.form {
  text-align: center;
  list-style-type: none;
  padding: 0.2em 0.4em;
  display: flex;
  flex-direction: row;
  justify-content: center;
  border-radius: 10px;
  border: medium black ridge;
  width: 13em;
  text-decoration: none;
  background: deepskyblue;

  color: black;
  text-shadow: 0px 0px 3px white, 0 0 5px grey;
}

.form a {
}

/* bloc volets: menu, articles, a-side*/
.volets {
  display: flex;
  flex-direction: row;
  justify-content: center;
  margin: 0.25em;
}

.menu,
section,
footer {
  padding: 0% 0.25em;
  margin: 0% 0.25em;
}

nav {
  margin: 0px 0.5em 0px auto;
  flex-direction: column;
  justify-content: flex-start;
  text-align: center;
  list-style: none inside;
  word-break: auto;
  text-shadow: 0px 0px 3px white, 0 0 5px grey;
  background: rgba(255, 255, 255, 0.15);
}

li {
  padding-bottom: 4px;
}

.menu {
  color: black;
  display: block;
  width: 8em;
  padding: 0.3em;
  text-decoration: none;
  text-overflow: auto;
  /*
		background: teal;
		border: medium black outset;
		border-radius: 6px;
		*/
}

ul li {
  list-style: '- ' inside;
  text-indent: -0.5em;
}

ol li {
  list-style: inside decimal;
  text-indent: -0.5em;
}

section {
  margin: 0% auto;
  padding: 0.5em;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  width: auto;

  border-radius: 0.5em;
  background: teal;
}

section h1 {
  text-indent: 3em;
}

section h2 {
  text-indent: 2em;
}
section h3 {
  text-indent: 1em;
}

article {
  text-indent: 1em;
  background: skyblue;
  text-align: justify;
  border-radius: inherit;
  padding: 0.5em;
  margin: 0.5em;
}

/*
article ul li {
  list-style-image: url('img/fleche16.png');
}
*/

#renvoi {
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
  padding: 1em;
}

aside {
}

article h3 {
  column-span: all;
  -webkit-column-span: all;
  -moz-column-span: all;
}

section,
article {
  column-count: 3;
  -webkit-column-count: 3;
  -moz-column-count: 3;
  break-before: auto;
  break-after: auto;
  break-inside: avoid-column;
  -moz-break-before: auto;
  -moz-break-after: auto;
  -moz-break-inside: avoid-column;
  -webkit-break-before: auto;
  -webkit-break-after: auto;
  -webkit-break-inside: avoid-column;

  hyphens: auto;
  -webkit-hyphens: auto;
  -moz-hyphens: auto;
  column-rule: 1px dotted;
  -webkit-column-rule: 1px dotted;
  -moz-column-rule: 1px dotted;
  column-gap: 2em;
  -webkit-column-gap: 2em;
  -moz-column-gap: 2em;
}

a,
.form {
  cursor: hand;
}
a:hover,
footer li:hover {
  text-shadow: 0 0 5px lime, 0 0 7px white;
  -webkit-transform: rotate(180deg) 1s;
  transition: transform 3.5s ease-out;
  transform: rotateX(-3600deg) skew(0deg, 0deg) translate(0px, 0em) scale(1.25);
  /*
		animation: heartbeat 0.7s;
	}
		@keyframes heartbeat {
			0% {}
			20% {transform: scale(1.5);}
			40% {transform: scale(1.25);}
			60% {transform: scale(1.25);}
			80% {transform: scale(1.5);}


			100%{}
		*/
}
.form:hover {
  transition: transform 3.5s ease-out;
  transform: rotateX(-3600deg) skew(0deg, 0deg) translate(0px, 0em) scale(1);
}

a:focus,
footer li:focus {
  transition: transform 5s ease;
  transform: rotateX(0deg) skew(0deg, 0deg) translate(0px, 0em) scale(0.01)
    alternate;
}

/*pied de page*/
footer {
  background: lightgrey;

  margin: 0% auto;
  vertical-align: bottom;
  border: medium black ridge;
  border-radius: 6px;
}

footer ul {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  vertical-align: bottom;
}

footer ul li {
  list-style-type: none;
}

footer ul li a {
  color: black;
  text-decoration: none;
  text-shadow: 0px 0px 4px white;
}
</style>
