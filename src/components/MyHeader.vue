<template>

  <div class="container">
    <a>
      <img id="logo" src="../assets/img/dc-logo.png" alt="">
    </a>

    <nav>
      <ul>
        <a class="listItems">CHARACTERS</a>
        <a class="listItems">COMICS</a>
        <a class="listItems">MOVIES</a>
        <a class="listItems">TV</a>
        <a class="listItems">GAMES</a>
        <a class="listItems">COLLECTIBLES</a>
        <a class="listItems">VIDEOS</a>
        <a class="listItems">FANS</a>
        <a class="listItems">NEWS</a>
        <a class="listItems">SHOP</a>
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
    margin: 0px auto;
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

  .listItems{
    list-style: none;
    font-size: 12px;
    font-weight: 700;
    padding: 50px 0px;
    border-bottom: 5px solid $DcColor-none;

    &:hover, &:active{
      border-bottom: 5px solid $DcColor-active;
    } 
  }

</style>