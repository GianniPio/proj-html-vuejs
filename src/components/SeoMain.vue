<template>
    <main>
      <ChiSiamo/>
      <CosaFacciamo/>
      <DoveLavoriamo/>
    </main>
</template>

<script>

import ChiSiamo from "@/components/ChiSiamo.vue"
import CosaFacciamo from "@/components/CosaFacciamo.vue"
import DoveLavoriamo from "@/components/DoveLavoriamo.vue"

export default {
  name: 'SeoMain',
  components: {
    ChiSiamo,
    CosaFacciamo,
    DoveLavoriamo
  }
}
</script>

<style scoped lang="scss">


</style>
