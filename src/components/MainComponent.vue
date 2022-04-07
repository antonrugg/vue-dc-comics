<template>

  <main>
    <div class="jumbotron">
      
    </div>
    <div class="container-90w">
      <ProductItem v-for="(item, index) in products" :key="'prod-'+index" :pathImg="item.thumb" :typeProduct="item.type" :title="item.series"/>
    </div>
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
  padding-bottom: 5rem;

  .jumbotron{
    background-image: url('@/assets/img/jumbotron.jpg');
    height: 53vh;
  }

  .container-90w{
        display: flex;
        justify-content: space-between;
        align-items: center;
      }
}

</style>