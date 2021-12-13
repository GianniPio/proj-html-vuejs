<template>
    <!-- hedaer -->
    <header>

        <!-- logo -->
        <div id="logo">
            <img src="../../src/assets/images/logo_seo_w_1x.png" alt="Logo della pagina">
        </div>

        <!-- Menu -->
        <div id="menu">
         <Menu v-for="voice, i in menu" :key="i" :voices="voice"/>   
        </div>
        
        
        <!-- Bottone -->
        <button>
            <span>GET IN TOUCH NOW</span>
        </button>

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
    display: flex;
    justify-content: space-between;

    img {
    width: 100%;
    }

    #menu {

        display: inline-block;
        font-size: 15px;

    }

    button {
            height: 7%;
            line-height: 0%;
            padding: 20px;
            border-radius: 50px;
            background-color: orange;
            border: none;
            cursor: pointer;

            span {
                color: white;
                font-weight: bold;
            }
        } 
}



</style>
