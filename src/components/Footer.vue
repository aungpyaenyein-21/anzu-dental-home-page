<template>
  <section class="footer-warp d-flex justify-center align-center" 
    :style="$vuetify.breakpoint.xs?'height:160vh;width:100vw':'height:100vh;width:100vw;'"
  >
    <div :style="$vuetify.breakpoint.xs?'width:100vw':'width:80vw;'">
      <v-row>
        <v-col
          cols="12"
          sm="6"
          md="6"
          lg="6"
          :class=" $vuetify.breakpoint.xs?'d-flex flex-column justify-space-around align-start px-8':'d-flex flex-column justify-space-around align-start pa-10'"
        >
          <h1 class="pb-2">杏歯科医院<br>(あんずしかいいん)</h1>
          <h1>Address</h1>
          <p>〒168-0065 杉並区浜田山2-20-13 1F 京王井の頭線浜田山駅 徒歩1分</p>
          <iframe 
            src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d810.2045937431483!2d139.62663602936095!3d35.6814739!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x6018f23ed91c30dd%3A0x1578a3e207c9e4f0!2sAnzu%20Dental%20Clinic!5e0!3m2!1sen!2sjp!4v1647663634926!5m2!1sen!2sjp" 
            width="100%"
            height="350" 
            style="border: 5px double #B89355;" 
            allowfullscreen="" 
            loading="lazy">
          </iframe>
        </v-col>
        <v-col
          cols="12"
          sm="6"
          md="6"
          lg="6"
          :class=" $vuetify.breakpoint.xs?'d-flex flex-column justify-space-around align-start px-8':'d-flex flex-column justify-space-around align-start pa-10'"
        >
          <h1>Close</h1>
          <p>	金曜日、日曜日、祝日、臨時休診日</p>
          <h1>Open</h1>
          <p>月 - 木：10:00-13:00/14:00-18:00[最終受付17:00]</p>
          <p>土曜日：10:00-13:00/14:00-17:00[最終受付16:00]</p>
          <h1>Phone Number</h1>
          <p>03-5357-8170</p>
          <h1>Mail</h1>
          <p>info@dentallounge.jp</p>
          <h1>Dentist</h1>
          <p>森杏子</p>
          <h1>Follow Us</h1>
          <v-btn
            elevation="2"
            icon
            class="mt-2"
            color="white"
          >
            <v-icon color="white" size="20">mdi-instagram</v-icon>
          </v-btn>
        </v-col>
      </v-row>
      <div class="address">
        
      </div>
      <div class="infomation">
        
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Footer',
}
</script>

<style scoped>
  @import url('https://fonts.googleapis.com/css2?family=Noto+Sans+JP:wght@100;300;400;500;700;900&family=Noto+Serif+JP:wght@200;300;400;500;600;700;900&family=Playfair+Display:wght@600&family=Rampart+One&display=swap');
  @font-face {
    font-family: 'giaza';
    src: url(../fonts/Giaza.otf);
  }
  .footer-warp{
    /* height: 100vh; */
    width: 100vw;
    height: 100vh;
    background-color:#004736;
  }
  h1{
    font-family: 'giaza';
    color:#B89355;
    font-size: 1.3rem;
    letter-spacing: 3px;
  }
  p{
    font-family: 'Noto Sans JP', sans-serif;
    color:white;
    font-size: 1rem;
    letter-spacing: 3px;
  }
</style>