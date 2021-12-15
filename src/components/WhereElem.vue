<template>
    <div class="box">
        <!-- Prende i dati dell'array tramite le props -->
        <img :src="require(`../assets/images/${element}`)" :alt="index">
    </div>
</template>

<script>
export default {
  name: 'WhereElem',
  props: {
      element: String,
      index: String,
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
