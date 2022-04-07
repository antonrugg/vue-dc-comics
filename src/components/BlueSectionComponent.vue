<template>
  <section>
    <div class="container-80w">
       <div class="option-container">
         <img src="../assets/img/buy-comics-digital-comics.png" alt="digital comics">
         <a href="#nowhere">digital comics</a>
       </div>

       <div class="option-container">
         <img src="../assets/img/buy-comics-merchandise.png" alt="dc merchandise">
         <a href="#nowhere">dc merchandise</a>
       </div>

       <div class="option-container">
         <img src="../assets/img/buy-comics-subscriptions.png" alt="subscriptions">
         <a href="#nowhere">subscription</a>
       </div>

       <div class="option-container">
         <img src="../assets/img/buy-comics-shop-locator.png" alt="shop locator">
         <a href="#nowhere">comic shop locator</a>
       </div>

       <div class="option-container">
         <img src="../assets/img/buy-dc-power-visa.svg" alt="buy dc power visa">
         <a href="#nowhere">dc power visa</a>
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
        flex-wrap: wrap;
        column-gap: 1rem;
        

        .option-container{
          display: flex;
          justify-content: center;
          flex-basis: calc(100% / 6);
          align-items: center;
          padding: 4rem 0rem;
          flex-wrap: wrap;
          flex-grow: 1;
          transition: transform 0.3s;
          cursor: pointer;

            &:hover{
              transform: scale(1.3); 
              transition: 0.3s;
              transition-timing-function: linear;
            }
            
          

          img{
            max-height: 60px;
            max-width: 65px;
           

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