<script>
import navBar from './components/navBar.vue'
import contentMain from './components/contentMain.vue'
import contentFooter from './components/contentFooter.vue'



export default {
  components: {
    navBar, contentMain, contentFooter
  }
}
</script>

<template>

  <navBar />
  <contentMain />
  <contentFooter />
</template>

<style lang="scss">
@use "./components/styles/general.scss" as *;
</style>
