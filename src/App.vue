<template>
  <div id="app">
    <Header/>
    <SectionBlack/>
    <SectionBlue/>
  </div>
</template>

<script>

import Header from "./components/Header.vue"
import SectionBlack from "./components/SectionBlack.vue"
import SectionBlue from "./components/SectionBlue.vue"

export default {
  name: 'App',
  components: {
    Header,
    SectionBlack,
    SectionBlue,
  }
}
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
