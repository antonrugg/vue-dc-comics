<template>
    <article>
       <a href="#nowhere"><img :src="pathImg" :alt="typeProduct"></a>
       <a href="#nowhere"><p>{{title}}</p></a>
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
        flex-basis: calc(100% / 6);
        display: flex;
        flex-direction: column;
        align-items: center;
        flex-grow: 1;
        row-gap: 2rem;
        

        img{
            max-height: 100%;
            transition: transform 0.3s;

            &:hover{
                transform: scale(1.2);
                transition: transform 0.3s;
            }
        }


        a{

            text-decoration: none;
            color: white;

            &:hover{
                text-decoration: underline;
            }

            p{
            max-width: 200px;
            text-transform: uppercase;
            font-size: 14px;
            }
        }


        }
        

</style>