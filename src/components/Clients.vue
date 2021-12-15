<template>
    <section id="clients">

        <!-- Contenitore -->
        <div id="container">

            <!-- Parte di sopra -->
            <div class="sopra">
                <!-- Titolo -->
                <h1>
                    Whats Our Clients Say
                </h1>
            </div>

            <!-- Parte centrale -->
            <div class="centro">
                <!-- Prende i dati dell'array -->
                <div class="box active">
                    <img :src="require('../assets/images/'+boxs[clientActive].image)" :alt="boxs[clientActive].name">
                    <p class="italic">{{boxs[clientActive].text}}</p>
                    <p><span>{{boxs[clientActive].name}}</span>, {{boxs[clientActive].work}} </p>
                </div>
            </div>

            <div>
                <!-- Aggiunge la classe active tramite la funzione avanti o indietro -->
                <button :class="boxs[0].active === true ? 'active' : ''" @click="indietro"></button>
                <button :class="boxs[1].active === true ? 'active' : ''" @click="avanti"></button>
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
          boxs : [ // dati 
              {
                  image: "testimonials-1.jpg",
                  text: "Ability proceeds from a fusion of skills, knowledge,understanding and imagination, consolidated by experience.",
                  name: "Jennifer Lopez",
                  work: "FULL STACK DEVELOPER",
                  active: true
              },
              {
                  image: "testimonials-2.jpg",
                  text: "Ability proceeds from a fusion of skills, knowledge,understanding and imagination, consolidated by experience.",
                  name: "Luis Desalvo",
                  work: "CREO TECH",
                  active: false
              }
          ]
      }
  },
  methods: {

        avanti(){

            this.clientActive = 1;

            this.boxs[this.clientActive - 1].active = false,

            this.boxs[this.clientActive].active = true
            
        },

        indietro(){

            this.clientActive = 0;

            this.boxs[this.clientActive + 1].active = false,

            this.boxs[this.clientActive].active = true
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
            padding: 5% 0 5% 0;

            h1 {
                font-size: 30px;
            }
        }

        .centro {

            .box {
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
                background-color: black;
            }

            &.active {
                background-color: black;
            }
        }
    }
}
</style>
