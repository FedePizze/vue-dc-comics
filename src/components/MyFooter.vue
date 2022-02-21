<template>
  <div>
    <div id="list">
      <div class="container">

        <div id="leftBox">

          <div class="row">
            <h4>DC COMICS</h4>
            <nav>
              <ul>
                <li>Characters</li>
                <li>Comics</li>
                <li>Movies</li>
                <li>TV</li>
                <li>Games</li>
                <li>Videos</li>
                <li>News</li>
              </ul>
            </nav>

            <h4>SHOP</h4>
            <nav>
              <ul>
                <li>Shop DC</li>
                <li>Shop DC Collectibles</li>
              </ul>
            </nav>
          </div>

          <div class="row">
            <h4>DC</h4>
            <nav>
              <ul>
                <li>Terms Of Use</li>
                <li>Privacy policy (New)</li>
                <li>Ad Choices</li>
                <li>Advertising</li>
                <li>Jobs</li>
                <li>subscriptions</li>
                <li>Talent Workshop</li>
                <li>CPSC Cartificates</li>
                <li>Ratings</li>
                <li>Shop Help</li>
                <li>Contact Us</li>
              </ul>
            </nav>
          </div>

          <div class="row">
            <h4>SITES</h4>
            <nav>
              <ul>
                <li>DC</li>
                <li>MAD Magazine</li>
                <li>DC Kids</li>
                <li>DC Universe</li>
                <li>DC Power Visa</li>
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

      <div id="button">
        <h3 id="bottonText">SIGN-UP NOW!</h3>
      </div>

      <div id="socialBox">
        <h3 id="socialText">FOLLOW US</h3>
        <img class="socialImg" src="../assets/img/footer-facebook.png" alt="">
        <img class="socialImg" src="../assets/img/footer-twitter.png" alt="">
        <img class="socialImg" src="../assets/img/footer-youtube.png" alt="">
        <img class="socialImg" src="../assets/img/footer-pinterest.png" alt="">
        <img class="socialImg" src="../assets/img/footer-periscope.png" alt="">
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

  li{
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