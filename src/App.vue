<template>
  <MyHeader></MyHeader>
  <MyMain></MyMain>
  <MyFooter></MyFooter>
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MyMain from './components/MyMain.vue'
import MyFooter from './components/MyFooter.vue'

export default {
  name: 'App',
  components: {
    MyHeader,
    MyMain,
    MyFooter
  }
}
</script>

<style lang="scss">
  @import "./assets/style/elements.scss";


</style>
