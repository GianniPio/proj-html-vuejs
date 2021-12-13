<template>
    <!-- hedaer -->
    <header>

        <!-- logo -->
        <div id="logo">
            <img src="../../src/assets/images/logo_seo_w_1x.png" alt="Logo della pagina">
        </div>

        <!-- Menu -->
        <div id="menu">
            <ul>
                <li v-for="voice, i in menu" :key="i">
                    <a :href="voice.link">{{voice.title}}</a>
                </li>
            </ul>
        </div>
        
        <!-- Bottone -->
        <button>
            <span>GET IN TOUCH NOW</span>
        </button>

    </header>

    
</template>

<script>

export default {
  name: 'SeoHeader',

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
        font-size: 13px;

        li {
            display: inline;
            padding: 20px;

            a {
                color: white;
                text-decoration: none;

                &:hover {
                color: orange;
                }
            }


           
        }
    }

    button {
            margin-top: -10px;
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
