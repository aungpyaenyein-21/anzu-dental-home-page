<template>
  <v-app style="position: relative;">
    <div class="nav-bar">
      <div class="logo">
        <router-link to="/">Logo</router-link>
      </div>
      <div class="menu" @click="openMenuDialog">
        <span class="bar1"></span>
        <span class="bar2"></span>
        <span class="bar3"></span>
      </div>
    </div>
    <v-main  class="main">
      <router-view/>
    </v-main>
    <div class="menu-dialog">
      <ul>
          <li><a  href="#">Treatment</a></li>
          <li><a @click="closeMenuDialog" href="#"><router-link to="/booking">Booking</router-link></a></li>
          <li><a href="#">Gallery</a></li>
          <li><a href="#">Staff</a></li>
          <li><a href="#">Contact</a></li>
      </ul>
    </div>
  </v-app>
</template>

<script>

import gsap from 'gsap'
export default {
  name: 'App',

  data: () => ({
    menuDialog:false,
  }),

  watch:{
    $route(newVal){
      if(newVal){
        this.closeMenuDialog()
      }
    }
  },

  methods:{
    openMenuDialog(){
      const tl = gsap.timeline()
      if(this.menuDialog === false){
        gsap.to('.bar1',{duration:.2,width:'45px',height:'6px',top:'45%',rotate:'45deg'})
            gsap.to('.bar3',{duration:.2,width:'45px',height:'6px',top:'45%',rotate:'-45deg'})
            gsap.to('.bar2',{duration:.2,opacity:0})

            tl.to('.main',{duration:.5,opacity:0,display:'none'})
            tl.to('.menu-dialog',{duration:.5,opacity:1,display:'block'})
            tl.to('li',{duration:.1,opacity:1,y:10,stagger:.1})
            this.menuDialog = true;
        }else{
            tl.to('li',{duration:.1,opacity:0,y:-10,stagger:.1})
            tl.to('.menu-dialog',{duration:.5,opacity:0,display:'none'})
            tl.to('.main',{duration:.5,opacity:1,display:'block'})
            gsap.to('.bar1',{duration:.2,width:'37px',height:'5px',top:'25%',rotate:'0deg'})
            gsap.to('.bar3',{duration:.2,width:'37px',height:'5px',top:'65%',rotate:'0deg'})
            gsap.to('.bar2',{duration:.2,opacity:1})
            this.menuDialog = false
      }
    },
    closeMenuDialog(){
      const tl = gsap.timeline()
      tl.to('li',{duration:.1,opacity:0,y:-10,stagger:.1})
      tl.to('.menu-dialog',{duration:.5,opacity:0,display:'none'})
      tl.to('.main',{duration:.5,opacity:1,display:'block'})
      gsap.to('.bar1',{duration:.2,width:'37px',height:'5px',top:'25%',rotate:'0deg'})
      gsap.to('.bar3',{duration:.2,width:'37px',height:'5px',top:'65%',rotate:'0deg'})
      gsap.to('.bar2',{duration:.2,opacity:1})
      this.menuDialog = false
    }
    
  }

};
</script>

<style scoped>
  .nav-bar{
      position: fixed;
      width: 100%;
      height: 60px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      top: 0;
      left: 0;
      padding: 10px;
      z-index: 10;
  }
  .nav-bar .menu{
      position: relative;
      height: 65px;
      width: 65px;
      cursor: pointer;
      z-index: 1;
      transition: .3s ease-in-out;
  }
  .bar1, .bar2, .bar3{
      position: absolute;
      display: inline-block;
      transform: rotate(0deg);
      width: 37px;
      height: 5px;
      background-color: black;
      border-radius: 10px;
      transition: .3s ease-in-out;
  }
  .bar1{
      top: 25%;
  }
  .bar2{
      top: 45%;
  }
  .bar3{
      top: 65%;
  }
  .menu-dialog{
    position: absolute;
    width: 100%;
    height: 100vh;
    background-color: #efe7dd;
    opacity: 0;
    z-index: 0;
    display: none ;
  }
  .menu-dialog ul{
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%,-50%);
      list-style: none;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
  }
  .menu-dialog li{
      font-size: 3rem;
      margin: 1rem 0;
      /* font-style: italic; */
      font-weight: bold;
      letter-spacing: 3px;
      opacity: 0;
  }
  .menu-dialog a{
      color: rgb(85, 44, 33);
      text-decoration: none;
      text-transform: uppercase;
  }
  .menu-dialog a:hover{
            
      font-size: 3.1rem;
      transition: .3s ease-in-out;
      position: relative; 
      top: -3px; 
      left: -3px; 
      text-shadow: 1px 1px #ffffff, 
                  2px 2px #ffffff, 
                  3px 3px#ffffff, 
                  4px 4px #ffffff, 
                  5px 5px #ffffff, 
                  6px 6px #ffffff;
  }

</style>
