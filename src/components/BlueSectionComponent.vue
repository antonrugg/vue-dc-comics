<template>
  <section>
    <div class="container-80w">
       <div class="option-container">
         <img src="../assets/img/buy-comics-digital-comics.png" alt="digital comics">
         <a href="#nowehre">digital comics</a>
       </div>

       <div class="option-container">
         <img src="../assets/img/buy-comics-merchandise.png" alt="dc merchandise">
         <a href="#nowehre">dc merchandise</a>
       </div>

       <div class="option-container">
         <img src="../assets/img/buy-comics-subscriptions.png" alt="digital comics">
         <a href="#nowehre">subscription</a>
       </div>

       <div class="option-container">
         <img src="../assets/img/buy-comics-shop-locator.png" alt="digital comics">
         <a href="#nowehre">comic shop locator</a>
       </div>

       <div class="option-container">
         <img src="../assets/img/buy-dc-power-visa.svg" alt="digital comics">
         <a href="#nowehre">dc power visa</a>
       </div> 
    </div> 
  </section>
</template>

<script>
export default {
    name: 'BlueSectionComponent',
}
</script>

<style lang="scss" scoped>

section{
  background-color: rgb(12 124 236);

  .container-80w{
        display: flex;
        justify-content: space-between;
        align-items: center;
        flex-wrap: no-wrap;
        

        .option-container{
          display: flex;
          align-items: center;
          padding: 4rem 0rem;
          flex-wrap: wrap;
          flex-grow: 1;
          

          img{
            max-height: 60px;
            max-width: 65px;
            margin-right: 0.7rem;
          }

          a{
            color: white;
            text-decoration: none;
            text-transform: uppercase;
            font-size: 14px;
            

            &:hover{
              text-decoration: underline;
            }
          }
        }
      }
}


</style>