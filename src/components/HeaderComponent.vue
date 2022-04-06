<template>

  <header>
    <div class="container-90w">
      <img src="../assets/img/dc-logo.png" alt="DC logo">
      <div id="menu-container">
        <ul>
          <li><a href="#nowhere">characters</a></li>
          <li><a href="#nowhere">comics</a></li>
          <li><a href="#nowhere">movies</a></li>
          <li><a href="#nowhere">tv</a></li>
          <li><a href="#nowhere">games</a></li>
          <li><a href="#nowhere">collectibles</a></li>
          <li><a href="#nowhere">videos</a></li>
          <li><a href="#nowhere">fans</a></li>
          <li><a href="#nowhere">news</a></li>
          <li><a href="#nowhere">shop</a></li>
        </ul>
      </div>
      </div>
  </header>
  
</template>

<script>
export default {
    name: 'HeaderComponent',
}
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
                color: blue;
                border-bottom: 3px solid blue;
                padding-bottom: 3.425rem;
              }
            }

          
        }
      }



    }


</style>
