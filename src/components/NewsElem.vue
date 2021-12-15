<template>
    <!-- Prende i dati dell'array tramite la props -->
    <div class="box">
        <img :src="require(`../assets/images/${element.image}`)" :alt="element.title">
        <span class="title">{{element.title}}</span>
        <span class="data">{{element.date}}</span>
        <p>{{element.text}}</p>
    </div>
</template>

<script>
export default {
  name: 'NewsElem',
  props: {
      element: Object,
  }
}
</script>

<style scoped lang="scss">
.box {

    margin: 10px;
    text-align: center;

    img {
        width: 100%;
    }

    .title {
        font-weight: bold;
        font-size: 13px;
        color: orange;
        display: block;
    }

    .data {
        font-size: 10px;
        padding-bottom: 10px;
        display: inline-block;
    }

    p {
        line-height: 130%;
        font-size: 15px;
        color: grey;
    }
}
</style>