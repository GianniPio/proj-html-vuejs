<template>
    <main>
      <Who/>
      <What/>
      <Where/>
      <Plans/>
      <News/>
    </main>
</template>

<script>

import Who from "@/components/Who.vue"
import What from "@/components/What.vue"
import Where from "@/components/Where.vue"
import Plans from "@/components/Plans.vue"
import News from "@/components/News.vue"

export default {
  name: 'SeoMain',
  components: {
    Who,
    What,
    Where,
    Plans,
    News
  }
}
</script>

<style scoped lang="scss">

</style>
