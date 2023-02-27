<script>

import Appheader from './components/AppHeader.vue';
import contents from './components/AppContents.vue';
import AppFooter from './components/AppFooter.vue';

export default {

  components: {
    Appheader,
    contents,
    AppFooter
  }
}
</script>

<template>
  <Appheader />
  <contents />
  <AppFooter />
</template>

<style scoped></style>
