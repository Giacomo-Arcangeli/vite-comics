<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppFooterTop from './components/AppFooterTop.vue'
import AppFooterBottom from './components/AppFooterBottom.vue'
export default {
  components: { AppHeader, AppMain, AppFooterTop, AppFooterBottom },
  data() {
    return
  }
}
</script>

<template>
  <div>
    <AppHeader />
    <AppMain />
    <AppFooterTop />
    <AppFooterBottom />
  </div>
</template>

<style>
/* reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* generics */

body {
  font-family: 'Montserrat', sans-serif;
  font-family: 'Open Sans', sans-serif;
}

li {
  list-style-type: none;
}

img {
  height: auto;
  max-width: 100%;
}

a {
  color: black;
  text-decoration: none;
}

/* utilities */
.container {
  max-width: 1400px;
  margin: 0 auto;
}
</style>