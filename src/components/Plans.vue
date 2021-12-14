<template>
    <div id="plans">
        <div class="container">

            <div class="sopra">
                <h2>
                    Our Plans
                </h2>
                <p>
                    Sed ut perspiciatis unde omnis natus error sit voluptatem accusantium doloremque laudantium.
                </p>
            </div>

            <div class="centro">
                <PlansElem v-for="box, i in boxs" :key="i" :element="box"/>
            </div>

        </div>
    </div>
</template>

<script>
 
import PlansElem from "@/components/PlansElem.vue"

export default {
  name: 'Plans',
  components: {
      PlansElem
  },
  data() {
      return {
          boxs : [
              {
                  title: "Standard",
                  price: "19",
                  note1: "5 Projects",
                  note2: "5 GB Storage",
                  note3: "Unlimited Users"
              },
              {
                  title: "Premium",
                  price: "29",
                  note1: "10 Projects",
                  note2: "15 GB Storage",
                  note3: "Unlimited Users"
              },
              {
                  title: "Professional",
                  price: "39",
                  note1: "15 Projects",
                  note2: "30 GB Storage",
                  note3: "Unlimited Users"
              },
              {
                  title: "Extreme",
                  price: "59",
                  note1: "Unlimited Projects",
                  note2: "Unlimited Storage",
                  note3: "Unlimited Users"
              }
          ]
      }
  }
}
</script>

<style scoped lang="scss">

#plans {
    background-image: url("../../src/assets/images/background1.jpg");
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center;

    .container {
        width: 70%;
        margin: 0 auto;
        text-align: center;

        .sopra {
            width: 60%;
            margin: 0 auto;
            padding: 5% 0 10% 0;
            color: white;

            h2 {
                font-size: 30px;
                padding-bottom: 2%;
            }

            p {
                font-weight: bold;
            }
        }
    }
}

</style>
