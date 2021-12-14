<template>
    <section id="clients">

        <div id="container">

            <div class="sopra">
                <h1>
                    Whats Our Clients Say
                </h1>
            </div>

            <div class="centro">
                <div class="box active">
                    <img :src="boxs[clientActive].image" :alt="boxs[clientActive].name">
                    <p class="italic">{{boxs[clientActive].text}}</p>
                    <p><span>{{boxs[clientActive].name}}</span>, {{boxs[clientActive].work}} </p>
                </div>
            </div>

            <div>
                <button @click="indietro"></button>
                <button @click="avanti"></button>
            </div>
        </div>
    </section>
</template>

<script>


export default {
  name: 'Clients',
  data() {
      return {
          clientActive: 0,
          boxs : [
              {
                  image: "../../src/assets/images/testimonials-1.jpg",
                  text: "Ability proceeds from a fusion of skills, knowledge,understanding and imagination, consolidated by experience.",
                  name: "Jennifer Lopez",
                  work: "FULL STACK DEVELOPER",
                  active: true
              },
              {
                  image: "../../src/assets/images/testimonials-1.jpg",
                  text: "Ability proceeds from a fusion of skills, knowledge,understanding and imagination, consolidated by experience.",
                  name: "Luis Desalvo",
                  work: "CREO TECH",
                  active: true
              }
          ]
      }
  },
  methods: {
        avanti(){

            this.clientActive = 1;
            
        },

        indietro(){

            this.clientActive = 0;
        }

    
    }
}
</script>

<style scoped lang="scss">

#clients {
    background-color: white;
    height: auto;
    

    #container {
        width: 70%;
        margin: 0 auto;
        border-bottom: 1px solid lightgray;
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
        }

        .centro {

            .box {
                margin: 10px;
                text-align: center;
                display: none;

                &.active {
                    display: block;
                }

                img {
                    width: 10%;
                    border-radius: 50%;
                }

                p {
                    line-height: 130%;
                    font-size: 15px;

                    &.italic {
                    font-style: italic;
                    padding-bottom: 15px;
                    }
                    
                    span {
                        font-weight: bold;
                    }
                }
            }
        }

        button {
            padding: 5px;
            border: 1px solid black;
            margin: 10px;
            border-radius: 50%;
            background-color: white ;
            cursor: pointer;

            &:hover {
                border: 1px solid red;
            }
        }
    }
}
</style>
