<template>
    <footer>
      <Logo/>
      <Consult/>
      <Copyright/>
    </footer>
</template>

<script>

import Logo from "@/components/Logo.vue/"
import Consult from "@/components/Consult.vue/"
import Copyright from "@/components/Copyright.vue"

export default {
  name: 'SeoFooter',
  components: {
    Logo,
    Consult,
    Copyright
  }
}
</script>

<style scoped lang="scss">
footer {
  height: 300px;
  padding-top: 50px;  
}
</style>
