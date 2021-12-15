<template>
  <div>
    <!-- Header della pagina -->
    <SeoHeader/>
    <!-- main della pagina -->
    <SeoMain/>

    <!-- Footer della pagina -->
    <SeoFooter/>
  </div>
</template>

<script>
// Componenti importati
import SeoHeader from './components/SeoHeader.vue'
import SeoMain from './components/SeoMain.vue'
import SeoFooter from './components/SeoFooter.vue'

export default {
  name: 'App',
  components: {
    SeoHeader,
    SeoMain,
    SeoFooter,
  }
}
</script>

<style lang="scss">

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
