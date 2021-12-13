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
    background-color: purple;
    height: 600px;
    padding: 2% 10%;

    #sopra {

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

                span {
                    color: white;
                    font-weight: bold;
                }
            } 
        }

        
    }

    

    
}



</style>
