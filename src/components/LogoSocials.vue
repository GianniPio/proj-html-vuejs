<template>
    <li>
        <a :href="logo.link">
            <i :class="logo.font"></i>
        </a>
    </li>
</template>

<script>
export default {
  name: 'LogoSocials',
  props: {
      logo: Object
  }
}
</script>

<style scoped lang="scss">


li {

    margin: 0 15px;

    a {
        color: black;

        &:hover {
            color: orange;
        }
    }
}


</style>
