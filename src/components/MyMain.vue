<template>

  <div id="content">
    <div id="jumbotron"></div>
  </div>

  <div id="comicsBox">

    <div class="container" id="load">
      <button class="serieButton"><h4>CURRENT SERIES</h4></button>
    </div>

    <div class="container" id="load">

      <ComicsCard
      v-for="(comic, index) in comics"
      :key="index"
      :img="comic.thumb"
      :name="comic.series"
      ></ComicsCard>
      <MyFooter></MyFooter>

    </div>

    <div class="container" id="load">
      <button class="loadButton">LOAD MORE</button>
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

import ComicsCard from './partials/ComicsCard.vue';

export default {
  name: 'MyMain',

  components: {
    ComicsCard
  },

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

      comics: [
        {
          thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
          price: "$19.99",
          series: "Action Comics",
          type: "comic book"
        },
        {
          thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
          pric: "$3.99",
          series: "American Vampire 1976",
          typ: "comic book"
        },
        {
          thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
          price: "$16.99",
          series: "Aquaman",
          type: "graphic novel"
        },
        {
          thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
          price: "$2.99",
          series: "Batgirl",
          type: "comic book"
        },
        {
          thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$3.99",
          series: "Batman",
          type: "comic book"
        },
        {
          thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$2.99",
          series: "Batman Beyond",
          type: "comic book"
        },
        {
          thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
          price: "$3.99",
          series: "Batman/Superman",
          type: "comic book"
        },
        {
          thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
          price: "$4.99",
          series: "Batman/Superman Annual",
          type: "comic book"
        },
        {
          thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
          price: "$5.99",
          series: "Batman: The Joker War Zone",
          type: "comic book"
        },
        {
          thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
          price: "$6.99",
          series: "Batman: Three Jokers",
          type: "comic book"
        },
        {
          thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
          price: "$4.99",
          series: "Batman: White Knight Presents: Harley Quinn",
          type: "comic book"
        },
        {
          thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
          price: "$16.99",
          series: "Catwoman",
          type: "graphic novel"
        }
      ]
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
    flex-wrap: wrap;
  }

  #content{
    align-items: center;
    background-color: $DcBlack;
    
    #jumbotron{
      width: 100%;
      height: 320px;
      background-image: url("../assets/img/jumbotron.jpg");
      background-position: top;
      background-size: cover;
    }
  }

  #comicsBox{
    background-color: $DcBlack;
    padding: 10px 0px;

    #load{
      justify-content: center;
      padding: 15px 0px;
      position: relative;
    }

    .loadButton{
      color: white;
      background-color: $DcColor-active;
      padding: 8px 55px;
      border: none;
    }

    .serieButton{
      color: white;
      background-color: $DcColor-active;
      padding: 8px 25px;
      border: none;
      position: absolute;
      left: 0;
      top: -33px;

      h4{
        font-size: 25px;
      }
    }
  }

  #points{
    align-items: center;
    background-color: $DcColor-active;

    .card{
      width: calc(100%/5);
      display: flex;
      justify-content: center;
      align-items: center;
      gap: 10px;
    }

    .linkText{
      font-size: 13px;
      color: white;
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

  }

  h2{
    font-size: 22px;
    color: white;
  }

</style>