<template>
    <div class="box">
        <img src="../../src/assets/images/case-study-gallery-3-1-1200x900.jpg" alt="Immagine">
        <img src="../../src/assets/images/case-study-gallery-2-1200x900.jpg" alt="Immagine">
        <img src="../../src/assets/images/case-study-gallery-1-1-1200x900.jpg" alt="Immagine">
        <img src="../../src/assets/images/case-study-gallery-4-1-1200x900.jpg" alt="Immagine">
        <img src="../../src/assets/images/case-study-gallery-5-1-1200x900.jpg" alt="Immagine">
        <img src="../../src/assets/images/case-study-gallery-6-1-1200x900.jpg" alt="Immagine">
    </div>
</template>

<script>
export default {
  name: 'WhereElem',
}
</script>

<style scoped lang="scss">
.box {

    text-align: center;
    width: 100%;

    img {
        width: calc(100% / 3.5);
        margin: 5px;
    }

}
</style>
