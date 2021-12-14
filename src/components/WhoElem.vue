<template>
    <div class="box">
        <i :class="element.icon"></i>
        <h6>{{element.title}}</h6>
        <p>{{element.text}}</p>
    </div>
</template>

<script>
export default {
  name: 'WhoElem',
  props: {
      element: Object,
  }
}
</script>

<style scoped lang="scss">
.box {

    background-color: white;
    margin: 10px;
    text-align: center;
    padding: 5%;

    i {
        color: #ffa837;
        font-size: 25px;
        padding-bottom: 10px;
        display: block;
    }

    h6 {
        font-weight: bold;
        font-size: 20px;
        padding-bottom: 10px;
    }

    p {
        line-height: 130%;
        font-size: 15px;
        color: grey;
    }
}
</style>
