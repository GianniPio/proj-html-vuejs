<template>
    <section id="cosa_facciamo">
        <img :src="require('../../src/assets/images/pattern_background.png')" alt="">

        <div id="container">

            <div class="sopra">
                <h1>
                    See Our Top Notch Services
                </h1>
                <p>
                    Sed ut perspiciatis unde omnis natus error sit voluptatem accusantium doloremque laudantium.
                </p>
            </div>

            <div class="centro">
                <WhatElem v-for="box, i in boxs" :key="i" :element="box"/>
            </div>

        </div>
    </section>
</template>

<script>

import WhatElem from "@/components/WhatElem.vue"

export default {
  name: 'What',
  components: {
      WhatElem,
  },
  data() {
      return {
          boxs : [
              {
                  icon: "fab fa-google",
                  title: "Google SEO",
                  text: "Vestibulum in lacinia metus. Suspendisse in enim ipsum. Nulla facilisi. Donec ante turpis, dictum sed magna et, dapibus faucibus odio.",
                  link: "Read more >"
              },
              {
                  icon: "fas fa-cog",
                  title: "Brand Strategy",
                  text: "Vestibulum in lacinia metus. Suspendisse in enim ipsum. Nulla facilisi. Donec ante turpis, dictum sed magna et, dapibus faucibus odio.",
                  link: "Read more >"
              },
              {
                  icon: "fas fa-building",
                  title: "Local SEO",
                  text: "Vestibulum in lacinia metus. Suspendisse in enim ipsum. Nulla facilisi. Donec ante turpis, dictum sed magna et, dapibus faucibus odio.",
                  link: "Read more >"
              },
              {
                  icon: "far fa-chart-bar",
                  title: "Seo Analysis",
                  text: "Vestibulum in lacinia metus. Suspendisse in enim ipsum. Nulla facilisi. Donec ante turpis, dictum sed magna et, dapibus faucibus odio.",
                  link: "Read more >"
              }
          ]
      }
  }
}
</script>

<style scoped lang="scss">

#cosa_facciamo {
    background-color: #051745;
    position: relative;

    img {
        width: 100%;
    }

    #container {
        width: 70%;
        margin: 0 auto;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);

        .sopra {
            text-align: center;
            width: 60%;
            margin: 5% auto;

            h1 {
                font-size: 30px;
                padding-bottom: 2%;
                color: white;
            }

            p {
                color: white;
                width: 60%;
                margin: 0 auto;
            }
        }

        .centro {
            display: flex;
            padding-bottom: 15%;

        }
    }
}
</style>
