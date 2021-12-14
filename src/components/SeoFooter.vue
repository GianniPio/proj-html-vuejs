<template>
    <footer>
      <Logo/>
      <Consult/>
    </footer>
</template>

<script>

import Logo from "@/components/Logo.vue/"
import Consult from "@/components/Consult.vue/"

export default {
  name: 'SeoFooter',
  components: {
    Logo,
    Consult
  }
}
</script>

<style scoped lang="scss">
footer {
  height: 300px;
  padding-top: 50px;  
}
</style>
