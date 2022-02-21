<template>

  <div id="content">
    <div class="container">
      <h2>-- Content goes here --</h2>
    </div>
  </div>

  <div id="points">
    <div class="container">
      <div class="card" v-for="(link, index) in links" :key="index">
        <img class="imgPoints" :src="link.src">
        <a class="linkText">{{link.text}}</a>
      </div>
      
    </div>

  </div>

</template>

<!-- --------------------------------------------------- --->

<script>

export default {
  name: 'MyMain',
  data() {
    return {
      links: [
          {
            text: "DIGITAL COMICS",
            src: "/img/buy-comics-digital-comics.png",
          },
          {
            text: "DC MERCHANDISE",
            src: "/img/buy-comics-merchandise.png",
          },
          {
            text: "SUBSCRIPTION",
            src: "/img/buy-comics-subscriptions.png",
          },
          {
            text: "COMIC SHOP LOCATOR",
            src: "/img/buy-comics-shop-locator.png",
          },
          {
            text: "DC POWER VISA",
            src: "/img/buy-dc-power-visa.svg",
          },
      ],
    }
  }
}
</script>

<!-- --------------------------------------------------- --->

<style scoped lang="scss">
  @import "../assets/style/variables.scss";

  .container{
    width: 70%;
    padding: 40px 0px;
    margin: 0px auto;
    display: flex;
  }

  #content{
    align-items: center;
    background-color: $DcBlack;
  }

  #points{
    align-items: center;
    background-color: $DcColor-active;
  }

  .card{
    width: calc(100%/5);
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 10px;
  }

  .imgPoints{
    width: 39px;
  }

  .card:nth-child(1) .imgPoints{
    width: 32px;
  }

  .card:nth-child(4) .imgPoints{
    width: 22px;
  }

  h2{
    font-size: 22px;
    color: white;
  }

  .linkText{
    font-size: 13px;
    color: white;
  }

</style>