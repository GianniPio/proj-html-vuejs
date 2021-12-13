<template>
  <div>
    <SeoHeader/>
    <SeoMain/>
  </div>
</template>

<script>
import SeoHeader from './components/SeoHeader.vue'
import SeoMain from './components/SeoMain.vue'

export default {
  name: 'App',
  components: {
    SeoHeader,
    SeoMain
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
