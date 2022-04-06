<template>

  <header>
    <div class="container-90w">
      <img src="../assets/img/dc-logo.png" alt="DC logo">
      <div id="menu-container">
        <ul>
          <li v-for="link in menus" :key="link"><a href="#nowhere">{{link}}</a></li>
        </ul>
      </div>
      </div>
  </header>
  
</template>

<script>
export default {
  name: "HeaderComponent",
  data() {
    return {
      menus: ["characters", "comics", "movies", "tv", "games", "collectibles", "video", "fans", "news", "shop"]
    };
  },
};
</script>




<style lang="scss" scoped>

    header{
      background-color: white;
      
      .container-90w{
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 1rem 0rem;
      }

      ul{
        display: flex;
        list-style-type: none;

        li{
          padding: 0rem 0.8rem;
          font-weight: 600;
          font-size: 16px;
          text-transform: uppercase;
          

            a{
              color: gray;
              text-decoration: none;

               &:hover{
                color: rgb(12 124 236);
                border-bottom: 5px solid rgb(12 124 236);
                padding-bottom: 3.325rem;
              }
            }

          
        }
      }



    }


</style>
