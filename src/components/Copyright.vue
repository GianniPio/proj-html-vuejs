<template>
    <div id="container">

        <div id="logo">
            <img src="../../src/assets/images/logo_seo_2x.png" alt="Logo Seo">
        </div>

        <div id="menu">
            <ul>
               <MenuFooter v-for="voice, i in menu" :key="i" :voices="voice"/> 
            </ul>
            
        </div>

        <div id="copy">
            <p>&copy; Copyright 2012 - 2020 | Awada Theme by <b>ThemeFusion</b> | All Rights Reserved | Powered by <b>WordPress</b></p>
        </div>

        <div id="social">
            <ul>
                <LogoSocials v-for="logos, i in logoSocials" :key="i" :logo="logos"/>
            </ul>
        </div>
    </div>
</template>

<script>

import MenuFooter from '@/components/MenuFooter.vue'
import LogoSocials from "@/components/LogoSocials.vue"

export default {

  name: 'Copyright',
  components: {
        MenuFooter,
        LogoSocials
    },
  data() {
    return {
        menu : [
            {
                title: "Home",
                link: "#",
            },

            {
                title: "Who We Are",
                link: "#chi_siamo",
            },

            {
                title: "What We Do",
                link: "#cosa_facciamo",
            },

            {
                title: "Where We Work",
                link: "#dove_lavoriamo",
            },

            {
                title: "Carrers",
                link: "#plans",
            },

            {
                title: "News",
                link: "#news",
            }
        ],

        logoSocials: [
            
                {
                    font: "fab fa-facebook-f",
                    link: "https://www.facebook.com/avadaspace"
                },

                {
                    font: "fab fa-instagram",
                    link: "https://www.instagram.com/avadaspace/"
                },

                {
                    font: "fab fa-twitter",
                    link: "https://twitter.com/avadaspace"
                },

                {
                    font: "fab fa-youtube",
                    link: "https://www.youtube.com/channel/UCir5t-mfvaul-JMIdKYtiGA"
                }
        ]
    }

  }
}
</script>

<style scoped lang="scss">

#container{
    width: 70%;
    margin: 2% auto;

    #logo {
        width: 10%;
        margin: 0 auto; 
        
        img{
            width: 100%;
            margin: 10% auto;
        }
    }

    #copy {

        text-align: center;
        margin-bottom: 2%;

        p {
            font-size: 12px;
        }
    }

    ul {
        display: flex;
        justify-content: center;
        list-style-type: none;
        padding: 3% 0;
    }


   
}

</style>
