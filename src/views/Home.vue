<template>
  <div class="home">

    <!-- <div class="header">
      <img id="banner" src="../assets/banner.png" alt="">
    </div> -->

    <img id="img-pic" alt="me logo" src="../assets/me.jpg">
    <HelloWorld msg="Jose A. Juarez"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  }
}
</script>

<style scoped>

#banner{
width: 100%;
  height: auto;
}

#img-pic{
  margin-top: 50px;
  width:200px;
}
</style>
