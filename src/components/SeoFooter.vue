<template>
    <footer>
      <Logo/>
    </footer>
</template>

<script>

import Logo from "@/components/Logo.vue/"

export default {
  name: 'SeoFooter',
  components: {
    Logo
  }
}
</script>

<style scoped lang="scss">
footer {
  height: 300px;
  padding-top: 50px;  
}
</style>
