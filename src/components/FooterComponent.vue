<template>
  <footer>
      <div class="container-90w">
        <div class="list-container">
          <ul>
            <li>dc comics</li>
            <li><a href="#nowhere">Characters</a></li>
            <li><a href="#nowhere">Comics</a></li>
            <li><a href="#nowhere">Movies</a></li>
            <li><a href="#nowhere">TV</a></li>
            <li><a href="#nowhere">Games</a></li>
            <li><a href="#nowhere">Videos</a></li>
            <li><a href="#nowhere">News</a></li>
          </ul>

          <ul>
            <li>shop</li>
            <li><a href="#nowhere">Shop DC</a></li>
            <li><a href="#nowhere">Shop DC Collectibles</a></li>
          </ul>
        </div>

        <div class="list-container">
          <ul>
            <li>dc</li>
            <li><a href="#nowhere">Terms Of Use</a></li>
            <li><a href="#nowhere">Privacy policy (News)</a></li>
            <li><a href="#nowhere">Ad Choices</a></li>
            <li><a href="#nowhere">Advertising</a></li>
            <li><a href="#nowhere">Jobs</a></li>
            <li><a href="#nowhere">Subscriptions</a></li>
            <li><a href="#nowhere">Talent Workshops</a></li>
            <li><a href="#nowhere">CPSC Certificates</a></li>
            <li><a href="#nowhere">Ratings</a></li>
            <li><a href="#nowhere">Shop Help</a></li>
            <li><a href="#nowhere">Contact Us</a></li>
          </ul>
        </div>

        <div class="list-container">
          <ul>
            <li>sites</li>
            <li><a href="#nowhere">DC</a></li>
            <li><a href="#nowhere">MAD Magazine</a></li>
            <li><a href="#nowhere">DC Kids</a></li>
            <li><a href="#nowhere">DC Universe</a></li>
            <li><a href="#nowhere">DC Power Visa</a></li>
          </ul>
        </div> 
      </div>

      
      <div class="social-container">
        <a class="btn" href="#nowhere">sign-up now!</a>
        <div class="icons">
          <span>follow us</span>
          <a href="#nowhere"><img src="../assets/img/footer-facebook.png" alt="facebook icon"></a>
          <a href="#nowhere"><img src="../assets/img/footer-twitter.png" alt="twitter icon"></a>
          <a href="#nowhere"><img src="../assets/img/footer-youtube.png" alt="youtube icon"></a>
          <a href="#nowhere"><img src="../assets/img/footer-pinterest.png" alt="pinterest icon"></a>
          <a href="#nowhere"><img src="../assets/img/footer-periscope.png" alt="periscope icon"></a>
        </div>
      </div>

  </footer>
</template>

<script>
export default {
    name: 'FooterComponent',
}
</script>

<style lang="scss" scoped>


  footer{
    background-image: url('../assets/img/dc-logo-bg.png'), url('../assets/img/footer-bg.jpg');
    background-position: right bottom, left top;
    background-size: 500px 450px, 100% 100%;
    background-repeat: no-repeat;
    background-origin: content-box;
    overflow-x: hidden;
    // height: 50vh;

  .container-90w{
  display: flex;
  justify-content: flex-start;
  align-items: flex-start;
    
    

    .list-container{
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      // max-width: 40%;
      margin-right: 8%;
      padding-top: 1.5rem;

      ul{
        display: flex;
        flex-direction: column;
        justify-content: space-evenly;
        align-items: flex-start;
        margin-bottom: 1.5rem;
        list-style-type: none;

        li{
          color: grey;
          padding: 0.3rem;
          font-size: 14px;

          a{
            text-decoration: none;
            color: grey;

            &:hover{
              text-decoration: underline;
              color: white;
            }
          }

          &:first-of-type{
            font-size: 18px;
            font-weight: 700;
            text-transform: uppercase;
            color: white;
          }
        }
      }

      

      }

      
    }

.social-container{
      
      background-color: rgb(48 48 48);
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 1rem 100px;  
      column-gap: 1rem;

     a.btn{
        color: white;
        font-size: 16px;
        padding: 1rem 2rem;
        border: 2px solid rgb(12 124 236);
        text-decoration: none;
        text-transform: uppercase;

        &:hover{
          background-color: rgb(12 124 236);
          transition: 0.3s;
        }
      }

      span{
        text-transform: uppercase;
        font-size: 16px;
        font-weight: 700;
        color: rgb(12 124 236);
        vertical-align: middle;
        
      }

     .icons{
       display: flex;
       justify-content: flex-start;
       align-items: center;
       flex-wrap: wrap;
       row-gap: 0.5rem;
       column-gap: 0.5rem;
         
        img{
        vertical-align: middle;
        color: rgb(12 124 236);
        padding: 0rem 0.5rem;
        
          &:hover{
            transform: scale(1.2);
            transition: 0.3s;
          }
        }
       
        
     } 
     


    }
    
  }

</style>