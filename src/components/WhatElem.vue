<template>
    <div class="box">
        <!-- Prende i dati dell'array tramite la prop -->
        <i :class="element.icon"></i>
        <h6>{{element.title}}</h6>
        <p>{{element.text}}</p>
        <a href="#">{{element.link}}</a>
    </div>
</template>

<script>
export default {
  name: 'WhatElem',
  props: {
      element: Object,
  }
}
</script>

<style scoped lang="scss">
.box {

    background-color: #1a236c;
    margin: 10px;
    text-align: center;
    padding: 5%;
    color: white;

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
        width: 50%;
        margin: 0 auto;
    }

    p {
        line-height: 130%;
        font-size: 15px;
        color: grey;
        padding-bottom: 20px;
        color: white;
    }

    a {
        color: orange;
        text-decoration: none;
    }
}
</style>
