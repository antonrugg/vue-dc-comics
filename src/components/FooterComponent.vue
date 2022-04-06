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
    background-size: 500px 450px, 100%;
    background-repeat: no-repeat;
    background-origin: content-box;
    display: flex;
    height: 50vh;

  .container-90w{
  display: flex;
  justify-content: flex-start;
  align-items: flex-start;

    .list-container{
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      margin-right: 4rem;

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
  }

</style>