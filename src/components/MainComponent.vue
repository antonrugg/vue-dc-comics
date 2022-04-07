<template>

  <main>
    <div class="jumbotron">
      <div id="jumbo-label"><p>current series</p></div>
    </div>
    <div class="container-90w">
      <ProductItem v-for="(item, index) in products" :key="'prod-'+index" :pathImg="item.thumb" :typeProduct="item.type" :title="item.series"/>
      

    </div>
   <a id="load-more-btn" href="#nowhere">load more</a>
    
  </main>

</template>

<script>

import ProductItem from '@/components/ProductItem.vue'

export default {
    name: 'MainComponent',

     props: {
        products: Array
    },
    components: {
         ProductItem
    }
}
</script>

<style lang="scss" scoped>

main{
  background-color: black;
  color: white;
  padding-bottom: 2rem;
  text-align: center;

  .jumbotron{
    background-image: url('@/assets/img/jumbotron.jpg');
    background-position: center top;
    height: 53vh;
    position: relative;

    #jumbo-label{
      position: absolute;
      bottom: -15px;
      left: 125px;
      padding: 0.3rem 2rem;
      background-color: rgb(12, 124, 236);
      color: white;
      text-align: center;
      vertical-align: middle;
      text-transform: uppercase;
      font-size: 24px;
      font-weight: 900;
      transform:scaleY(1.5)

    }

   
  }

  .container-90w{
        display: flex;
        justify-content: flex-start;
        align-items:flex-start;
        flex-wrap: wrap;
        row-gap: 2rem;
        padding-top: 4rem;
        margin-bottom: 4rem;
      }


   #load-more-btn{
      background-color: rgb(12, 124, 236);
      padding: 0.7rem 4rem;
      color: white;
      font-size: 12px;
      font-weight: 800;
      text-decoration: none;
      text-transform: uppercase;

        &:hover{
            opacity: 0.8;
            transition: 0.3s;
        }
     

      
    }
}

</style>