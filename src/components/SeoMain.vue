<template>
    <main>
      <Who/>
      <What/>
      <Where/>
    </main>
</template>

<script>

import Who from "@/components/Who.vue"
import What from "@/components/What.vue"
import Where from "@/components/Where.vue"

export default {
  name: 'SeoMain',
  components: {
    Who,
    What,
    Where
  }
}
</script>

<style scoped lang="scss">


</style>
