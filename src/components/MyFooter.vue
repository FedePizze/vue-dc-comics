<template>
  <div>
    <div id="list">
      <div class="container">

        <div id="leftBox">

          <div class="row">
            <h4>DC COMICS</h4>
            <nav>
              <ul>
                <a>Characters</a>
                <a>Comics</a>
                <a>Movies</a>
                <a>TV</a>
                <a>Games</a>
                <a>Videos</a>
                <a>News</a>
              </ul>
            </nav>

            <h4>SHOP</h4>
            <nav>
              <ul>
                <a>Shop DC</a>
                <a>Shop DC Collectibles</a>
              </ul>
            </nav>
          </div>

          <div class="row">
            <h4>DC</h4>
            <nav>
              <ul>
                <a>Terms Of Use</a>
                <a>Privacy policy (New)</a>
                <a>Ad Choices</a>
                <a>Advertising</a>
                <a>Jobs</a>
                <a>subscriptions</a>
                <a>Talent Workshop</a>
                <a>CPSC Cartificates</a>
                <a>Ratings</a>
                <a>Shop Help</a>
                <a>Contact Us</a>
              </ul>
            </nav>
          </div>

          <div class="row">
            <h4>SITES</h4>
            <nav>
              <ul>
                <a>DC</a>
                <a>MAD Magazine</a>
                <a>DC Kids</a>
                <a>DC Universe</a>
                <a>DC Power Visa</a>
              </ul>
            </nav>
          </div>

        </div>

  

        <div id="rightBox">

        </div>

      </div>
    </div>
    
  </div>



  <div id="footer">

    <div class="container">

      <a id="button">
        <h3 id="bottonText">SIGN-UP NOW!</h3>
      </a>

      <div id="socialBox">
        <h3 id="socialText">FOLLOW US</h3>
        <a href=""><img class="socialImg" src="../assets/img/footer-facebook.png" alt=""></a>
        <a href=""><img class="socialImg" src="../assets/img/footer-twitter.png" alt=""></a>
        <a href=""><img class="socialImg" src="../assets/img/footer-youtube.png" alt=""></a>
        <a href=""><img class="socialImg" src="../assets/img/footer-pinterest.png" alt=""></a>
        <a href=""><img class="socialImg" src="../assets/img/footer-periscope.png" alt=""></a>
      </div>   

    </div>

  </div>
  
</template>

<!-- --------------------------------------------------- --->

<script>

export default {
  name: 'HelloWorld',

}
</script>

<!-- --------------------------------------------------- --->

<style scoped lang="scss">
  @import "../assets/style/variables.scss";

  .container{
    width: 70%;
    margin: 0px auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  #leftBox{
    display: flex;
    align-items:flex-start;
    color: white;
    gap: 35px;
  }

  #list{
    background-image: url("../assets/img/footer-bg.jpg");
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
  }

  #rightBox{
    width: 550px;
    height: 370px;
    background-image: url("../assets/img/dc-logo-bg.png");
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
  }

  h4{
    margin-top: 50px;
  }

  .row{
    margin-bottom: 50px;
  }

  nav{
    margin-top: 10px;
  }

  ul{
    display: flex;
    flex-direction:column;
  }

  a{
    list-style: none;
    color: gray;
    font-size: 12px;
    padding: 2px 0px;
  }



  

  #footer{
    background-color: #303030;
    padding: 20px 0px;
  }

  #bottonText{
    color: white;
    border: 3px solid $DcColor-active;
    font-size: 15px;
    font-weight: 400;
    padding: 6px 10px;
  }

  #socialText{
    color: $DcColor-active;
    font-size: 15px;
    font-weight: 700;
  }

  #socialBox{
    display: flex;
    gap: 15px;
    align-items: center;
  }

  .socialImg{
    width: 30px;
  }

</style>