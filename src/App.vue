<script>
import AppHeader from "./components/AppHeader.vue"
import AppMain from "./components/AppMain.vue"
import AppFooter from "./components/AppFooter.vue"
import AppFasciaAzzurra from "./components/AppFasciaAzzurra.vue"

export default {
  components: {
    AppHeader,
    AppMain,
    AppFooter,
    AppFasciaAzzurra,
  }
}
</script>
<template lang="">
  <div>
    <AppHeader/>
    <AppMain/>
    <AppFasciaAzzurra/>
    <AppFooter/>

  </div>
</template>
<style lang="scss">
@use "./styles/partials/variables" as *;
@use "./styles/generals.scss" as *;
</style>