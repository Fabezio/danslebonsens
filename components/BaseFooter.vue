<template lang="pug">
footer
  p.semibold.text-center.uppercase dans le bon sens&nbsp;
    span.medium &copy; {{new Date().getFullYear()}}
  ul.flex.justify-center
    li.mx-2 LIVRE D'OR
    li.mx-2 NEWS
    li.mx-2 CONTACTS
    li.mx-2 FAQ
    li.mx-2 CGU
    li.mx-2 LIENS
    a.uppercase(href="https://github.com/Fabezio/danslebonsens") mon code source

</template>

<script>
export default {}
</script>

<style scoped>
footer {
  position: absolute;
  bottom: 0;
  width: 100%;
  padding: 0% 0.25em;
  margin: 0% 0.25em;
  background: lightgrey;

  vertical-align: bottom;
  border-radius: 6px;
  /*
  border: medium black ridge;
  */
}

ul {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  vertical-align: bottom;
}

ul li {
  list-style-type: none;
}

ul li:hover {
  /*
  text-shadow: 0 0 5px lime, 0 0 7px white;
  -webkit-transform: rotate(180deg) 1s;
  transition: transform 3.5s ease-out;
  transform: rotateX(-3600deg) skew(0deg, 0deg) translate(0px, 0em) scale(1.25);

    */
}
ul li a {
  color: black;
  text-decoration: none;
  text-shadow: 0px 0px 4px white;
}
li:focus {
  transition: transform 5s ease;
  transform: rotateX(0deg) skew(0deg, 0deg) translate(0px, 0em) scale(0.01)
    alternate;
}
</style>
