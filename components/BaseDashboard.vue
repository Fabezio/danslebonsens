<template lang="pug">
nav
  .flex.justify-between.mx-2
    .menu.mx-2(v-for='(link, index) in links', :key='index')
      nuxt-link(:to=`link.route`) {{link.label}}

</template>

<script>
export default {
  data() {
    return {
      links: [
        { route: '/', label: 'accueil' },
        { route: '/civilite', label: 'civilité' },
        { route: '/culture', label: 'culture' },
        { route: '/education', label: 'éducation' },
        { route: '/evolution', label: 'évolution' },
        { route: '/informatique', label: 'informatique' }
      ]
    }
  }
}
</script>

<style scoped>
nav {
  text-shadow: 0px 0px 3px white, 0 0 5px grey;
  background: rgba(255, 255, 255, 0.15);
  /*
  margin: 0px 0.5em 0px auto;
  text-align: center;
  list-style: none inside;
  word-break: auto;
  */
}
.menu {
  color: black;
  display: block;
  text-decoration: none;
  text-overflow: auto;
  font-size: 1.5em;
  width: 8em;
  /*
  padding: 0% 0.25em;
  margin: 0% 0.25em;
  padding: 0.3em;
		background: teal;
		border: medium black outset;
		border-radius: 6px;
		*/
}
.menu:hover {
  /*
  text-decoration: underline;
  */
  text-shadow: none;
  color: white;
  font-weight: 500;
}
</style>
