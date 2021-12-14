<template>
    <div id="logo">
        <div class="container">
            <LogoImages v-for="image, i in images" :key="i" :logo="image"/>
        </div>
    </div>
</template>

<script>

import LogoImages from "@/components/LogoImages.vue"

export default {
  name: 'Logo',
  components: {
      LogoImages
  },
  data() {
      return {
          images: [
              {
                  url: "clients_partner_5-200x202.png",
                  name: "avada_1"
              },
              {
                  url: "clients_partner_6-200x202.png",
                  name: "avada_2"
              },
              {
                  url: "clients_partner_1-200x202.png",
                  name: "avada_3"
              },
              {
                  url: "clients_partner_2-200x202.png",
                  name: "avada_4"
              }
          ]
      }
  }
}
</script>

<style scoped lang="scss">

#logo {
    background-color:white;

    .container {
        width: 70%;
        margin: 0 auto;
    }
}

</style>
