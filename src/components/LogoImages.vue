<template>
    <div class="box">
        <img :src="require(`../assets/images/${logo.url}`)" :alt="logo.name">
    </div>
</template>

<script>
export default {
  name: 'LogoImages',
  props: {
      logo: Object,
  }
}
</script>

<style scoped lang="scss">
.box {
    margin: 0 2.5%;
    text-align: center;
    width: 20%;
    display: inline-block;

    img {
        width: 100%;
        padding: 25%;
    }
}
</style>