<template>
    <section id="news">

        <!-- Contenitore -->
        <div id="container">

            <!-- Parte di sopra -->
            <div class="sopra">
                <!-- Titolo -->
                <h1>
                    Our News
                </h1>
                <!-- Paragrafo -->
                <p>
                    Sed ut perspiciatis unde omnis natus error sit voluptatem accusantium doloremque laudantium.
                </p>
            </div>

            <!-- Parte centrale -->
            <div class="centro">
                <!-- Prende gli elementi di NewsElem, in base all'array -->
                <NewsElem v-for="box, i in boxs" :key="i" :element="box"/>
            </div>

            <button>GO TO NEWS</button>

        </div>
    </section>
</template>

<script>

import NewsElem from "@/components/NewsElem.vue"

export default {
  name: 'News',
  components: {
      NewsElem
  },
  data() {
      return {
          boxs : [  //array per la stampa dei box
              {
                  image: "related-service-2-700x441.jpg",
                  title: "Why You Need A SEO Agency Now",
                  date: "November 1st, 2017",
                  text: "ALorem ipsum dolor sit amet, consectetur adepiscing elit. In et scelerisque sem. Nunc molestie neque augue, at gravida mi blandit."
              },
              {
                  image: "related-service-4-700x441.jpg",
                  title: "SEO Tips For Your Startup",
                  date: "November 1st, 2017",
                  text: "ALorem ipsum dolor sit amet, consectetur adepiscing elit. In et scelerisque sem. Nunc molestie neque augue, at gravida mi blandit."
              },
              {
                  image: "blog-post-6-700x441.jpg",
                  title: "Image Optimization For Your Site",
                  date: "November 1st, 2017",
                  text: "ALorem ipsum dolor sit amet, consectetur adepiscing elit. In et scelerisque sem. Nunc molestie neque augue, at gravida mi blandit."
              }
          ]
      }
  }
}
</script>

<style scoped lang="scss">

#news {
    background-color: #f8f8f8;
    height: auto;

    #container {
        width: 70%;
        margin: 0 auto;
        text-align: center;

        .sopra {
            text-align: center;
            width: 60%;
            margin: 0 auto;
            padding: 5% 0 10% 0;

            h1 {
                font-size: 30px;
                padding-bottom: 2%;
            }

            p {
                color: grey;
                font-weight: bold;
                width: 70%;
                text-align: center;
                margin: 0 auto;
            }
        }

        .centro {
            display: flex;
        }

        button {
            background-color: #ffa837;
            border-radius: 20px;
            padding: 10px;
            border: none;
            color: white;
            margin: 10px 0 50px 0;

            &:hover{
                filter: brightness(0.5);
            }
        }
    }
}
</style>
