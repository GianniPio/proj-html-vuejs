<template>
    <div class="box">
        <!-- Prende i dati dell'array tramite la props -->
        <h6>{{element.title}}</h6>
        <p>
            <sup>$</sup>
            <span class="price blu">{{element.price}}</span>
            <sup class="blu">99</sup>
            <sub>monthly</sub>
        </p>

        <p>{{element.note1}}</p>
        <p>{{element.note2}}</p>
        <p>{{element.note3}}</p>

        <button>START TODAY</button>
    </div>
</template>

<script>
export default {
  name: 'PlansElem',
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
    display: inline-block;

    h6 {
        font-weight: bold;
        font-size: 20px;
        padding-bottom: 10px;
    }

    p {
        padding-bottom: 15px ;
        font-size: 15px;

        .blu {
            color: cornflowerblue;
            font-weight: bold;
        }

        .price {
            font-size: 30px;
        }
    }

    button {
        background-color: white;
        border-radius: 20px;
        padding: 10px;
        border: 1px solid black;

        &:hover {
            background-color: orange;
            border: none;
            margin: 1px;
        }
    }
}
</style>