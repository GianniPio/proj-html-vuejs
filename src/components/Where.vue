<template>
    <section id="dove_lavoriamo">

        <!-- Contenitore -->
        <div id="container">

            <!-- Parte di sopra -->
            <div class="sopra">
                <!-- Titolo -->
                <h1>
                    Our Work
                </h1>
                <!-- Paragrafo -->
                <p>
                    Sed ut perspiciatis unde omnis natus error sit voluptatem accusantium doloremque laudantium.
                </p>
            </div>

            <!-- Parte centrale -->
            <div class="centro">
                <!-- Prende gli elementi di WhereElem, in base all'array -->
                <WhereElem v-for="image, i in images" :key="i" :element="image" :index="i"/>
            </div>

            <!-- Bottone -->
            <div class="sotto">
                <button>VIEW OUR WORK</button>
            </div>

        </div>
    </section>
</template>

<script>

import WhereElem from "@/components/WhereElem.vue"

export default {
  name: 'Where',
  components: {
      WhereElem,
  },
    data() {
        return {
            images : [
                "case-study-gallery-3-1-1200x900.jpg",
                "case-study-gallery-2-1200x900.jpg",
                "case-study-gallery-1-1-1200x900.jpg",
               "case-study-gallery-4-1-1200x900.jpg",
               "case-study-gallery-5-1-1200x900.jpg",
               "case-study-gallery-6-1-1200x900.jpg"
            ]
        }
    }
}
</script>

<style scoped lang="scss">

#dove_lavoriamo {
    background-color: #f8f8f8;
    height: auto;
    text-align: center;

    #container {
        width: 70%;
        margin: 0 auto;

        .sopra {
            text-align: center;
            width: 60%;
            margin: 0 auto;
            padding: 5% 0;

            h1 {
                font-size: 30px;
                padding-bottom: 2%;
            }

            p {
                color: grey;
                font-weight: bold;
            }
        }

        button {
        background-color: orange;
        border: none;
        border-radius: 20px;
        color: white;
        padding: 1%;
        margin: 5% 0;

        &:hover {
            filter: brightness(0.5);
        }
        }
    }
}
</style>
