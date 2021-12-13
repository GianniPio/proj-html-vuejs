<template>
    <!-- hedaer -->
    <header>
        <!-- Parte di sopra -->
        <div id="sopra">
            <!-- logo -->
            <div id="logo">
                <img src="../../src/assets/images/logo_seo_w_1x.png" alt="Logo della pagina">
            </div>

            <!-- Menu -->
            <div id="menu">
            <Menu v-for="voice, i in menu" :key="i" :voices="voice"/>

            <!-- Bottone -->
            <button>
                <span>GET IN TOUCH NOW</span>
            </button>
            </div>
            
            
            
        </div>

        <!-- Parte di sotto -->
        <div id="sotto">
            <div class="descr">
                <h1>
                    SEM Campaigns Made Simple With Avada
                </h1>
                <p>
                    Lorem ipsum dolor sit amet, consectetur adipisicing elit. Phasellus eu ornare erat. Curabitur pulvinar elit.
                </p>
                
                <button class="orange">BUY AVADA NOW</button>
                <button class="blue">CONTACTS US</button>

            </div>
        </div>
    </header>

    
</template>

<script>
import Menu from "@/components/Menu.vue"

export default {
  name: 'SeoHeader',
  components: {
    Menu,
  },

  data() {
    return {
        menu : [
            {
                title: "Home",
                link: "",
            },

            {
                title: "Who We Are",
                link: "",
            },

            {
                title: "What We Do",
                link: "",
            },

            {
                title: "Where We Work",
                link: "",
            },

            {
                title: "Carrers",
                link: "",
            },

            {
                title: "News",
                link: "",
            }
        ]
    }

  }

};

</script>

<style scoped lang="scss">


header {
    background-image: url("../../src/assets/images/1-hero-image.png");
    background-repeat: no-repeat;
    background-size: cover;
    height: 600px;
    padding: 2% 10%;

    #sopra {
        width: 100%;
        display: block;
        padding-bottom: 10%;

        img {
            width: 10%;
            float: left;
        }

        #menu {

            width: 90%;

            button {
                height: 7%;
                line-height: 0%;
                padding: 20px;
                border-radius: 50px;
                background-color: orange;
                border: none;
                cursor: pointer;
                float: right;

                &:hover {
                    filter: brightness(0.5)
                }

                span {
                    color: white;
                    font-weight: bold;
                }
            } 
        }
    }

    #sotto {
        width: 100%;

        .descr {
            width: 40%;
            color: white;

            h1 {
                font-size: 40px;
            }

            p {
                padding: 20px 0;
                font-size: 15px;
                color: lightgrey;

            }

            button {

                border-radius: 20px;
                padding: 3%;
                margin: 5px;
                border: none;
                color: white;
                font-weight: bold;
                cursor: pointer;
                font-size: 10px;

                &.orange {
                    background-color: #ffa837;
                }

                &.blue {
                    background-color: #0369d7;
                }

                &:hover {
                    filter: brightness(0.5)
                }
            }
        }

    }
 

    
}
</style>
