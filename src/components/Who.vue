<template>
    <section id="chi_siamo">

        <!-- Container -->
        <div id="container">

            <!-- Parte di sopra -->
            <div class="sopra">
                <!-- Titolo -->
                <h1>
                    Meet The New Agency SEO Template From The Avada Team
                </h1>
                <!-- Paragrafo -->
                <p>
                    Sed ut perspiciatis unde omnis natus error sit voluptatem accusantium doloremque laudantium.
                </p>
            </div>

            <!-- Parte centrale -->
            <div class="centro">
                <WhoElem v-for="box, i in boxs" :key="i" :element="box"/> <!-- stampa gli elementi che si trovano in WhoElem, in base all'array -->
            </div>

        <img src="../../src/assets/images/agency-seo-desk-front.jpg" alt="foto desktop">

        </div>
    </section>
</template>

<script>

import WhoElem from "@/components/WhoElem.vue"

export default {
  name: 'Who',
  components: {
      WhoElem
  },
  data() {
      return {
          boxs : [  //Array per la stampa dei box
              {
                  icon: "fas fa-road",
                  title: "Establish Goals",
                  text: "Aliquam non elit lacus. Praesent aliquet, ipsum id scelerisque convallis, mi liguia euismod odio, vel dictum mi risus a mi."
              },
              {
                  icon: "fas fa-video",
                  title: "Work With a Team",
                  text: "Cras semper auctor aliquam. Sed porta sed lacus sit amet consecteur. Lorem ipsum dolor sit amet, consectetur adipiscin."
              },
              {
                  icon: "fas fa-tint",
                  title: "Get Resutls",
                  text: "Vestibulum scelerisque egestas lectus sit amet molestie. Donec consectetur cursus est sed blandit. Nunc sed risus lacus."
              }
          ]
      }
  }
}
</script>

<style scoped lang="scss">

#chi_siamo {
    background-color: #f8f8f8;
    height: auto;

    #container {
        width: 70%;
        margin: 0 auto;

        .sopra {
            text-align: center;
            width: 60%;
            margin: 0 auto;
            padding: 5% 0 10% 0;

            h1 {
                font-size: 30px;
                padding-bottom: 2%;
                width: 80%;
                margin: 0 auto;
            }

            p {
                color: grey;
                font-weight: bold;
            }
        }

        .centro {
            display: flex;
        }

        img {
            width: 100%;
        }
    }
}
</style>
