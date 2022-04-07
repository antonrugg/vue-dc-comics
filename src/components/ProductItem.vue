<template>
    <article>
        <img :src="pathImg" :alt="typeProduct">
        <p>{{title}}</p>
    </article> 
</template>

<script>
export default {
     name: 'ProductItem',
     props: {
        product: Object,
        pathImg: String,
        title: String,
        typeProduct: String
    }
}
</script>

<style lang="scss" scoped>
    article{
        height: 250px;
        width: 200px;
    }

</style>