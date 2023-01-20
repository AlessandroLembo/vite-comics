<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  name: 'DC',
  data() {
    return {

    }

  },

  components: { AppHeader, AppMain, AppFooter }
}
</script>

<template>
  <app-header></app-header>
  <app-main></app-main>
  <app-footer></app-footer>

</template>

<style>
/* Reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* Generics */
body {
  font-family: "Open Sans", sans-serif;
}

img {
  max-width: 100%;
  height: auto;
}

a {
  text-decoration: none;
}
</style>