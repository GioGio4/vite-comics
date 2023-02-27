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

<style scoped></style>
