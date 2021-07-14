<template>
  <div class="hello">
    <h1>{{ msg }}</h1>


    <div id="my-links">
      <div class="container">
    
        <div class="col">
          <img class="site-pic" alt="me logo" src="../assets/logo.png">
          <button class="btn btn-light" onclick="window.open('https://josejuarez.netlify.app/', '_blank')">My Website</button>
        </div>

        <div class="col">
          <img class="site-pic" alt="me logo" src="../assets/linkedin.png">
          <button class="btn btn-light" onclick="window.open('https://www.linkedin.com/in/jose-a-juarez/', '_blank')">Linkedin</button>
        </div>

        <div class="col">
          <img class="site-pic" alt="me logo" src="../assets/insta.png">
          <button class="btn btn-light" onclick="window.open('https://www.instagram.com/eljosejuarez/', '_blank')">IG Photos</button>
        </div>

        <div class="col">
          <img class="site-pic" alt="me logo" src="../assets/twitter.png">
          <button class="btn btn-light" onclick="window.open('https://twitter.com/jo5ejuarez', '_blank')">Twitter</button>
        </div>
      </div>

      <div class="container" id="end-container">

        <div class="col">
          <img class="site-pic" alt="me logo" src="../assets/insta.png">
          <button class="btn btn-light" onclick="window.open('https://www.instagram.com/_themapache/', '_blank')">IG Gaming</button>
        </div>

        <div class="col">
          <img class="site-pic" alt="me logo" src="../assets/twitch.jpg">
          <button class="btn btn-light" onclick="window.open('https://www.twitch.tv/mapxche', '_blank')">Twitch</button>
        </div>

        <div class="col">
          <img class="site-pic" alt="me logo" src="../assets/yt.jpg">
          <button class="btn btn-light" onclick="window.open('https://www.youtube.com/channel/UCtie4UGB7rG41773hFIIjuw', '_blank')">YouTube</button>
        </div>

        <div class="col">
          <img class="site-pic" alt="me logo" src="../assets/discord.jpg">
          <button class="btn btn-light" onclick="window.open('https://discord.gg/2uAyeq7p7Y', '_blank')">Discord</button>
        </div>

      </div>
    
    </div>
    
    <div class="footer">
      <hr class="myhr">
      <div class="text">
        <p>© Copyrights 2021 Jose Juarez. All Rights Reserved</p>
      </div>
    </div>

  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class HelloWorld extends Vue {
  @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.hello{
   
  min-height: 72vh;
  display: flex;
  flex-direction: column;
}

h1{
  margin-bottom: 50px;
}

#my-links{
margin: auto 0px auto 0px ;
}

.container{
  display: flex;
  flex-wrap: wrap;
}

#end-container{
  margin-bottom: 50px;
}

.col{
  flex: 25%;
  justify-content: space-around;
}

.btn{
  width: 200px;
  padding: 25px 25px 25px 50px;
  color: black;
  background-color: white;
  border: 1px solid rgb(197, 197, 197);
  box-shadow: 4px 4px 1px rgba(0, 0, 0, 0.067);
  margin: 10px;
}

.site-pic{
  margin-top: 17px;
  width: 50px;
  position: absolute;
}

.footer{
  margin-top: auto;
  width: 100%;
  text-align: center;
  height: 180px;
}

hr.myhr{
   border: 1px solid rgb(231, 227, 227);
}

.text{
  margin-top: 70px;
}
</style>
