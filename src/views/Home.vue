<template>
  <div class="scroller pa-0" >
    <div class="welcomeWarp "
      :style="$vuetify.breakpoint.lg?'height: 130vh':'height: 100vh'" 
    >
      <div
        class="welcomeText d-flex flex-column justify-start align-center"
      > 
        <h1 data-scroll="" data-scroll-speed="2" 
        :style="$vuetify.breakpoint.lg?'font-size: 5rem;line-height: 200px;':'font-size: 2.5rem;line-height: 100px;'"
        >Welcome To The</h1>
        <h1 data-scroll="" data-scroll-speed="2" 
        :style="$vuetify.breakpoint.lg?'font-size: 5rem;line-height: 200px;':'font-size: 2.5rem;line-height: 100px;'" 
        >AnzuDental</h1>
        <h1 data-scroll="" data-scroll-speed="2" 
        :style="$vuetify.breakpoint.lg?'font-size: 5rem;line-height: 200px;':'font-size: 2.5rem;line-height: 100px;'" 
        >Clinic</h1>
      </div>
      
      <div class="smile-text">
        <h2 class="smile" 
          :style="$vuetify.breakpoint.lg?'font-size: 12rem':'font-size: 8rem'" 
        >SMILE</h2>
        <h2 class="everyday"
          :style="$vuetify.breakpoint.lg?'font-size: 12rem':'font-size: 5rem'" 
        >EVERYDAY</h2>
      </div>
      <div class="green-photo">
        <img :width="$vuetify.breakpoint.lg?'400':'200'" src="https://images.unsplash.com/photo-1556292026-bf74f176f6b2?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=MXwxfDB8MXxhbGx8fHx8fHx8fA&ixlib=rb-1.2.1&q=80&w=1080&utm_source=unsplash_source&utm_medium=referral&utm_campaign=api-credit" alt="">
      </div>
      <img class="bird" src="../assets/Swift2-.svg" width="100" alt="">
    </div>
    
    
    <div class="second-warp d-flex flex-column align-center">
      <img class="day" :width="$vuetify.breakpoint.lg?'40%':'60%'" src="https://aungpyaenyein-21.github.io/anzu/home.jpeg" alt="">
      <div class="mission">
        <!-- <h3 class="text-center">予防</h3> -->
        <p>私たちのクリニックでは、なんらかの症状が起きてしまう前に予防することを大切にしています。心地良い空間で口腔内ケアを楽しめるように。それが私達の願いです。</p>
        <!-- <p>心地良い空間で口腔内ケアを楽しめるように。</p>
        <p>それが私達の願いです。</p> -->
        
      </div>
      <div class="dental-lounge">
        <span>Fun Dental lounge</span>
        <span> For Prevention
        <v-icon size="30" color="#D2B48C">mdi-tooth-outline</v-icon></span>
      </div>
      <!-- <div class="prevention">
        For Prevention
        <v-icon size="30">mdi-tooth-outline</v-icon>
      </div> -->
    </div>
    <!-- <div class="imageWarp">
      <img class='close photo' src="../assets/close.jpg" alt="" >
      <img class="open photo" src="https://aungpyaenyein-21.github.io/anzu/home.jpeg" alt="">
    </div> -->
    <Footer/>
  </div>
</template>

<script>
  import Footer from '../components/Footer.vue'
  import locomotiveScroll from 'locomotive-scroll'
  import { gsap } from 'gsap';
  import { ScrollTrigger } from 'gsap/ScrollTrigger';
  export default {
    name: 'Home',

    components: {
      Footer
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

          gsap.from('.welcomeText h1',1,{
              opacity:0,y:'100px',stagger:.1
          })
          let Width = this.$vuetify.breakpoint.lg?'80%':'100%'
          gsap.to('.day',{
              width:Width,
              scrollTrigger:{
                  trigger:'.welcomeWarp',
                  start:'center top',
                  end:'80% top',
                  scroller: ".scroller",
                  // pin:true,
                  // markers:true,
                  scrub:true,
              }
          })
          gsap.from('.dental-lounge span',{
            opacity:0,stagger:.1,
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
          let Y = this.$vuetify.breakpoint.lg?1000:630
          let X = this.$vuetify.breakpoint.lg?1200:300
          gsap.to('.bird',3,{
            y:Y,x:X,
            scrollTrigger:{
              trigger:'.welcomeWarp',
              start:'top top',
              scroller: ".scroller",
              // pin:true,
              markers:true,
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
  @import url('https://fonts.googleapis.com/css2?family=Asset&family=Kiwi+Maru:wght@300&family=Playfair+Display:wght@600&display=swap');
  @font-face {
    font-family: 'brightwall';
    src: url(../fonts/Brightwall.ttf);
    fonst-style:normal;
    font-weight: 100;
  }
  @font-face {
    font-family: 'giaza';
    src: url(../fonts/Giaza.otf);
  }
  .welcomeWarp{
    /* height: 100vh; */
    position: relative;
    /* width: 100vw; */
    background-color: #F8F7F5;
  }
  .welcomeText{
    position: absolute;
    width: 100%;
    top: 30%;
    left: 50%;
    transform: translate(-50%,-30%);
    z-index: 2;
  }
  .welcomeText h1{
    font-family: 'brightwall';
    letter-spacing: 5px;
    
  }
  .green-photo{
    position: absolute;
    top: 0;
    left: 0;
    z-index: 0;
  }
  .smile-text{
    position: absolute;
    bottom: 0;
    left: 50%;
    transform: translateX(-50%);
    color: rgb(246, 225, 181);
    /* color: #FFEFCA; */
    z-index: 1;
  }
  .smile{
    font-family: 'giaza';
    /* font-size: 8rem; */
    letter-spacing: -5px;
    z-index: 1;
  }
  .everyday{
    font-family: 'giaza';
    /* font-size: 5rem; */
    letter-spacing: -5px;
    z-index: 1;
  }
  .second-warp{
    height: 100vh;
    background-color: #F8F7F5;
  }
  .mission{
    margin: 10px;
  }
  .mission p {
    font-family: 'Kiwi Maru', serif;
    color: rgb(85, 44, 33);
  }
  .mission h3{
    font-family: 'Kiwi Maru', serif;
    color: rgb(85, 44, 33);
  }
  .dental-lounge{
    font-size: 2.5rem;
    margin: 0 10px 0 10px;
    color: #D2B48C;
    font-family: 'giaza';
  }
  .bird{
    z-index: 3;
    position: absolute;
    top: -100px;
    left: -100px;
    transform: rotate(20deg);
  }
  /* .prevention{
    font-family: 'giaza';
    font-size: 2.5rem;
    margin: 0 10px 0 10px;
    color: rgb(85, 44, 33);
  } */
</style>
