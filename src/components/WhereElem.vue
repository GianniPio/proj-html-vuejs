<template>
    <div class="box">
        <img :src="require(`../assets/images/${element}`)" alt="Immagine">
    </div>
</template>

<script>
export default {
  name: 'WhereElem',
  props: {
      element: String,
  }
}
</script>

<style scoped lang="scss">
.box {

    width: calc(88% / 3);
    display: inline-block;
    margin: 15px;

    img {
        width: 100%;
    }

}
</style>
