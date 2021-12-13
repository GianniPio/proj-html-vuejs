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

ul {
    
    margin-left: 50px;
    list-style-type: none;
    

    li {
        float: left;
        padding: 30px;
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
    
}

</style>
