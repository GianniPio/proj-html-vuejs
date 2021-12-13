<template>
  <div>
    <SeoHeader/>
    <SeoMain/>
    <SeoFooter/>
  </div>
</template>

<script>
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
