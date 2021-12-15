<template>
    <li>
        <a :href="voices.link">{{voices.title}}</a>
    </li>
</template>

<script>
export default {
  name: 'Menu',
  props: {
    voices: Object,
  }
}
</script>

<style scoped lang="scss">

li {
    float: left;
    padding: 13px;
    font-size: 12px;

    a {
        color: #fff;
        font-weight: bold;
        text-decoration: none;

        &:hover {
            color: #ffa837
        }
    }
}

</style>
