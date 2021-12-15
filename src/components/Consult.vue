<template>
    <div id="consult">
        <div class="container">

            <div class="testo">
                <h2>
                    Start Your Free Consultation
                </h2>
                <p>
                    Sed ut perspiciatis unde omnis natus error sit voluptatem accusantium doloremque laudantium.
                </p>

                <button>CONTACT US NOW</button>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'Consult',
}
</script>

<style scoped lang="scss">

#consult {
    background-image: url("../../src/assets/images/case-study-gallery-3-1-1200x900.jpg");
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center;
    

    .container {
        width: 70%;
        margin: 0 auto;
        text-align: center;

        .testo {
            width: 60%;
            margin: 0 auto;
            padding: 10% 0;
            color: white;

            h2 {
                font-size: 30px;
                padding-bottom: 2%;
            }

            p {
                padding-bottom: 5%;
                width: 50%;
                margin: 0 auto;
            }

            button {
                background-color: #ffa837;
                color: white;
                border: none;
                padding: 2%;
                border-radius: 50px;
                font-weight: bold;

                &:hover {
                    filter: brightness(0.8);
                }
            }
        }
    }
}

</style>
