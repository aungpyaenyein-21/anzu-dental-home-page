<template>
  <v-container class="container pa-0" fluid>
    <div class="welcomeWarp d-flex flex-column justify-center align-center">
      <h1>Welcome</h1>
      <h1>To Anzu</h1>
      <h1>Dental</h1>
      <h1>Clinic</h1>
    </div>
    <div class="imageWarp">
      <img class="hero-img" src="https://aungpyaenyein-21.github.io/anzu/home.jpeg" alt="">
    </div>
  </v-container>
</template>

<script>
  // import HelloWorld from '../components/HelloWorld'

  export default {
    name: 'Home',

    components: {
      // HelloWorld,
    },
  }
</script>

<style scoped>
  @import url('https://fonts.googleapis.com/css2?family=Asset&family=Playfair+Display:wght@600&display=swap');
  .container{
    height: 200vh;
    
  }
  .welcomeWarp{
    height: 100vh;
    background-color: #efe7dd;
  }
  .welcomeWarp h1{
    font-family: 'Playfair Display';
    color: rgb(85, 44, 33);
    font-size: 80px;
    /* font-weight: 600; */
    line-height: 120px;
    letter-spacing: 5px;
  }
  .imageWarp{
    height: 100vh;
  }
  .hero-img{
    width: 100%;
  }
</style>
