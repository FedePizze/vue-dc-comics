<template>

  <div class="container">
    <a>
      <img id="logo" src="../assets/img/dc-logo.png" alt="">
    </a>

    <nav>
      <ul>
        <li>CHARACTERS</li>
        <li>COMICS</li>
        <li>MOVIES</li>
        <li>TV</li>
        <li>GAMES</li>
        <li>COLLECTIBLES</li>
        <li>VIDEOS</li>
        <li>FANS</li>
        <li>NEWS</li>
        <li>SHOP</li>
      </ul>
    </nav>
  </div>

</template>

<!-- --------------------------------------------------- --->

<script>

export default {
  name: 'MyHeader',

}
</script>

<!-- --------------------------------------------------- --->

<style scoped lang="scss">
  @import "../assets/style/variables.scss";

  .container{
    width: 70%;
    margin: 20px auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  #logo{
    width: 70px;
  }

  ul{
    display: flex;
    gap: 25px;
  }

  li{
    list-style: none;
    font-size: 12px;
    font-weight: 700;
    padding: 40px 0px;
    border-bottom: 5px solid $DcColor-none;

    &:hover, &:active{
      border-bottom: 5px solid $DcColor-active;
    } 
  }

</style>