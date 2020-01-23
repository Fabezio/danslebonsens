<template lang="pug">
header
  nav.flex.justify-between.bg-green-500.p-1.text-white.items-center
    nuxt-link.brand(to='/') DANS LE BON SENS
    BaseDashboard.btn.rounded.mx-3
    a.justify-end.form(href='../form.html') inscription/connexion

  h1.text-center.items-center DANS LE BON SENS
    br
    em Savoir c'est Devoir


</template>

<script>
export default {}
</script>

<style scoped>
header {
  height: 150px;
  text-align: center;
  border-radius: 10px;
  /*
  margin: 0.2em 0.4em;
  */
}
.brand {
  font-size: 1.5em;
  padding: 0.2em 0.4em;
  border-radius: 10px;
  /*
  border: medium black ridge;
  */
}
.home {
  /*
  width: 6em;
  list-style-type: none;
  */
}

.brand {
  text-decoration: none;
}
.form {
  cursor: hand;
  text-align: center;
  list-style-type: none;
  padding: 0 0.4em;
  border-radius: 10px;
  text-decoration: none;
  font-size: 1.5em;
  color: black;
  text-shadow: 0px 0px 3px white, 0 0 5px grey;
  /*
  background: deepskyblue;
  border: medium black ridge;
  width: 13em;
  display: flex;
  flex-direction: row;
  justify-content: center;
  */
}
/*
.form a {
  }
.form:hover {
  transition: transform 3.5s ease-out;
  transform: rotateX(-3600deg) skew(0deg, 0deg) translate(0px, 0em) scale(1);
}
*/
</style>
