<template>

    <li>
        <a :href="voices.link">{{voices.title}}</a>
    </li>

</template>

<script>
export default {
  name: 'MenuFooter',
  props: {
    voices: Object,
  }
}
</script>

<style scoped lang="scss">


    

li {
    padding: 13px;
    font-size: 12px;

    a {
        color: black;
        font-weight: bold;
        text-decoration: none;

        &:hover {
            color: #ffa837
        }
    }
}
    


</style>
