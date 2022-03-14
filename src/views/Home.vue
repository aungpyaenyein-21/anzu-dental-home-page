<template>
  <div class="scroller pa-0" >
    <div class="welcomeWarp d-flex flex-column justify-center align-center">
      <h1 data-scroll="" data-scroll-speed="2">Welcome To The</h1>
      <h1 data-scroll="" data-scroll-speed="2">AnzuDental</h1>
      <h1 data-scroll="" data-scroll-speed="2">Clinic</h1>
      <div class="smile-text">
        <div class="smile">SMILE</div>
        <div class="everyday">EVERYDAY</div>
      </div>
    </div>
    <div class="green-photo">
      <img width="200" src="https://images.unsplash.com/photo-1556292026-bf74f176f6b2?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=MXwxfDB8MXxhbGx8fHx8fHx8fA&ixlib=rb-1.2.1&q=80&w=1080&utm_source=unsplash_source&utm_medium=referral&utm_campaign=api-credit" alt="">
    </div>
    
    <div class="second-warp d-flex flex-column align-center">
      <img class="day" width="60%" src="https://aungpyaenyein-21.github.io/anzu/home.jpeg" alt="">
      <p>予防</p>
      <p>私たちのクリニックでは、なんらかの症状が起きてしまう前に予防することを大切にしています。</p>
      <p>心地良い空間で口腔内ケアを楽しめるように。</p>
      <p>それが私達の願いです。</p>
      <p>FUN！ Dental lounge For Prevention</p>
    </div>
    <!-- <div class="imageWarp">
      <img class='close photo' src="../assets/close.jpg" alt="" >
      <img class="open photo" src="https://aungpyaenyein-21.github.io/anzu/home.jpeg" alt="">
    </div> -->
  </div>
</template>

<script>
  import locomotiveScroll from 'locomotive-scroll'
  import { gsap } from 'gsap';
  import { ScrollTrigger } from 'gsap/ScrollTrigger';
  export default {
    name: 'Home',

    components: {
      // HelloWorld,
    },
    data() {
      return {
        x: null
      };
    },
    mounted(){
      this.setScroll();
    },
    methods:{
      setScroll() {
          let scroller = new locomotiveScroll({
              el:  document.querySelector('.scroller'),
              smooth: true,
              smoothMobile: true
          });
          gsap.registerPlugin(ScrollTrigger);
          scroller.on("scroll", ScrollTrigger.update);
          ScrollTrigger.scrollerProxy('.scroller', {
              scrollTop(value) {
                  return arguments.length
                      ? scroller.scrollTo(value, 0, 0)
                      : scroller.scroll.instance.scroll.y;
              },
              getBoundingClientRect() {
                  return {
                      left: 0,
                      top: 0,
                      width: window.innerWidth,
                      height: window.innerHeight
                  };
              },
          });

          gsap.from('.welcomeWarp h1',1,{
              opacity:0,y:'100px',stagger:.1
          })

          gsap.to('.day',{
              width:'100%',
              scrollTrigger:{
                  trigger:'.welcomeWarp',
                  start:'center top',
                  end:'80% top',
                  scroller: ".scroller",
                  // pin:true,
                  markers:true,
                  scrub:true,
              }
          })

          ScrollTrigger.addEventListener("refresh", () =>
              scroller.update()
          );
          ScrollTrigger.refresh();
      }
    }
  }
</script>

<style scoped>
  @import url('https://fonts.googleapis.com/css2?family=Asset&family=Playfair+Display:wght@600&display=swap');
  @font-face {
    font-family: 'brightwall';
    src: url(../fonts/Brightwall.ttf);
    fonst-style:normal;
    font-weight: 100;
  }
  .welcomeWarp{
    height: 100vh;
    position: relative;
    /* width: 100vw; */
    background-color: #F8F7F5;
  }
  .welcomeWarp h1{
    font-family: 'brightwall';
    /* color: rgb(85, 44, 33); */
    font-size: 2.5rem;
    /* font-weight: 600; */
    line-height: 100px;
    letter-spacing: 5px;
    z-index: 2;
  }
  .green-photo{
    position: absolute;
    top: 0;
    left: 0;
  }
  .smile-text{
    position: absolute;
    bottom: 0;
    left: 0;
    color: rgb(246, 225, 181);
  }
  .smile{
    font-family: 'Playfair Display';
    font-size: 8rem;
    letter-spacing: -5px;
  }
  .everyday{
    font-family: 'Playfair Display';
    font-size: 5rem;
    letter-spacing: -5px;
  }
  .second-warp{
    height: 100vh;
    background-color: #F8F7F5;
  }
  .imageWarp{
    height: 300vh;
    position: relative;
    background-color: aquamarine;
    overflow: hidden;
  }
  .photo{
    width: 100%;
    position: absolute;
    left: 0%;
    top: 0%;
    right: 0%;
    bottom: 0%;
    z-index: 1;
  }
  .open{
    z-index: 0;
  }
</style>
