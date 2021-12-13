<template>
    <section id="chi_siamo">

        <div id="container">

            <div class="sopra">
                <h1>
                    Meet The New Agency SEO Template From The Avada Team
                </h1>
                <p>
                    Sed ut perspiciatis unde omnis natus error sit voluptatem accusantium doloremque laudantium.
                </p>
            </div>

            <div class="centro"></div>

        <img src="../../src/assets/images/agency-seo-desk-front.jpg" alt="foto desktop">

        </div>
    </section>
</template>

<script>
export default {
  name: 'ChiSiamo',
}
</script>

<style scoped lang="scss">

#chi_siamo {
    background-color: #f8f8f8;

    #container {
        width: 60%;
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

        img {
            width: 100%;
        }
    }
}
</style>
