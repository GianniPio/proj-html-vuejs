<template>
    <section id="dove_lavoriamo">

        <div id="container">

            <div class="sopra">
                <h1>
                    Our Work
                </h1>
                <p>
                    Sed ut perspiciatis unde omnis natus error sit voluptatem accusantium doloremque laudantium.
                </p>
            </div>

            <div class="centro">
                <WhereElem/>
            </div>

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
            padding: 5% 0 10% 0;

            h1 {
                font-size: 30px;
                padding-bottom: 2%;
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

        button {
        background-color: orange;
        border: none;
        border-radius: 20px;
        color: white;
        padding: 1%;
        margin-bottom: 15px;

        &:hover {
            filter: brightness(0.5);
        }
        }
    }
}
</style>
