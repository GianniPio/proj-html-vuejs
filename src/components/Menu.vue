<template>
    <ul>
        <li>
            <a :href="voices.link">{{voices.title}}</a>
        </li>
    </ul>

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

    display: flex;
    padding: 20px;

    a {
        color: white;
        text-decoration: none;

        &:hover {
        color: orange;
        }
    }

}

</style>
