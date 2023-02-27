<script>

import AppHeader from './components/AppHeader.vue';
import AppContents from './components/AppContents.vue';
import AppFooter from './components/AppFooter.vue';

export default {

  components: {
    AppHeader,
    AppContents,
    AppFooter
  }
}
</script>

<template>
  <AppHeader />
  <AppContents />
  <AppFooter />
</template>

<style >
/* Reset */

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

img {
  max-width: 100%;
}

ul {
  list-style: none;
}

a {
  text-decoration: none;
  color: inherit;
}
</style>
