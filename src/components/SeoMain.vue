<template>
    <main>
      <ChiSiamo/>
      <CosaFacciamo/>
    </main>
</template>

<script>

import ChiSiamo from "@/components/ChiSiamo.vue"
import CosaFacciamo from "@/components/CosaFacciamo.vue"

export default {
  name: 'SeoMain',
  components: {
    ChiSiamo,
    CosaFacciamo,
  }
}
</script>

<style scoped lang="scss">


</style>
