<template>
    <main>
      <ChiSiamo/>
    </main>
</template>

<script>

import ChiSiamo from "@/components/ChiSiamo.vue"

export default {
  name: 'SeoMain',
  components: {
    ChiSiamo,
  }
}
</script>

<style scoped lang="scss">

main {
    height: 3000px;
    background-color: blue;
}

</style>
