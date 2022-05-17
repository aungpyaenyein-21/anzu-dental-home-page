<template>
  <div class="scroller">
    <div class="welcomeWarp"
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
      <div   class="green-photo">
        <img data-scroll="" data-scroll-speed="4" :width="$vuetify.breakpoint.lg?'400':'200'" src="https://aungpyaenyein-21.github.io/anzu-dental-photos/clinic-photos/leaf.jpg" alt="">
      </div>
      <img data-scroll="" data-scroll-speed="4" class="bird" src="https://aungpyaenyein-21.github.io/anzu-dental-photos/clinic-photos/bird.svg" width="100" alt="">
    </div>
    
    
    <div 
      class="second-warp d-flex justify-center align-center"
      :style="$vuetify.breakpoint.xs?'height:50vh':'height:100vh'" 
    >
      <img  
        class="day" 
        :width="$vuetify.breakpoint.xs?'100%':'80%'"
        src="https://aungpyaenyein-21.github.io/anzu-dental-photos/clinic-photos/home.jpeg" alt="">
    </div>
    <section 
      class="third-warp d-flex flex-column justify-center align-center"
      :style="$vuetify.breakpoint.xs?'height:50vh':'height:120vh'" 
    >
      <div class="dental-lounge d-flex flex-column justify-center align-center">
        <span :style="$vuetify.breakpoint.lg?'font-size: 5rem;line-height: 200px;':'font-size: 2rem;line-height: 80px;'">Fun Dental lounge</span>
        <span :style="$vuetify.breakpoint.lg?'font-size: 5rem;line-height: 200px;':'font-size: 2rem;line-height: 80px;'"> For Prevention
          <v-icon size="7vw" color="white">mdi-tooth</v-icon>
          <v-icon size="7vw" color="white">mdi-toothbrush</v-icon>
        </span>
      </div>
      <div class="mission d-flex flex-column justify-center align-center my-5">
        <!-- <h3 class="text-center">予防</h3> -->
        <h1 :style="$vuetify.breakpoint.xs?'font-size: 1rem;line-height: 30px;':'font-size: 1.5rem;line-height: 50px;'">私たちのクリニックでは、</h1>
        <h1 :style="$vuetify.breakpoint.xs?'font-size: 1rem;line-height: 30px;':'font-size: 1.5rem;line-height: 50px;'">なんらかの症状が起きてしまう前に</h1>
        <h1 :style="$vuetify.breakpoint.xs?'font-size: 1rem;line-height: 30px;':'font-size: 1.5rem;line-height: 50px;'">予防することを大切にしています。</h1>  
        <h1 :style="$vuetify.breakpoint.xs?'font-size: 1rem;line-height: 30px;':'font-size: 1.5rem;line-height: 50px;'">心地良い空間で口腔内ケアを楽しめるように。</h1>
        <h1 :style="$vuetify.breakpoint.xs?'font-size: 1rem;line-height: 30px;':'font-size: 1.5rem;line-height: 50px;'"> それが私達の願いです。</h1>
      </div>
    </section>
    
    <!-- our service -->
    <section
      :style="$vuetify.breakpoint.xs?'height:50vh;width:100vw':'height:100vh;width:100vw;'"
      class="our-services d-flex flex-column justify-center align-center"
    >
      <div 
        data-scroll="" 
        data-scroll-direction="horizontal" 
        data-scroll-speed="6" 
        class="service-outline"
        :style="$vuetify.breakpoint.xs?'fontSize:3rem;':'fontSize:11rem;'"
      >OUR SERVICES</div>
      <div 
        :style="$vuetify.breakpoint.xs?'fontSize:3rem;':'fontSize:11rem;'" 
        class="service"
      >OUR SERVICES</div>
      <div 
        data-scroll="" 
        data-scroll-direction="horizontal" 
        data-scroll-speed="-6"
        class="service-outline"
        :style="$vuetify.breakpoint.xs?'fontSize:3rem;':'fontSize:11rem;'" 
      >OUR SERVICES</div>
    </section>

    <!-- treatment1 -->
    <section 
      class="treatments treatment1 d-flex flex-column justify-center align-center" 
      :style="$vuetify.breakpoint.xs?'height:100vh;width:100vw;':'height:100vh;width:100vw;'"
    >
        <div class="circle-container">
          <div class="circ1"
            :style="$vuetify.breakpoint.xs?'height:600px;width:600px;':'height:700px;width:700px;'"
          ></div>
        </div>
        <h1
          class="my-10"
          :style="$vuetify.breakpoint.xs?'fontSize:2rem':'fontSize:3rem'"
        >一般歯科（保険治療）</h1>
        <div
          :style="$vuetify.breakpoint.xs?'width:100vw':'width:60vw'"
        >
        <v-row>
          <v-col
            cols="6"
            lg="4"
            md="4"
          >
            <div
              class="d-flex flex-column justify-start align-center"
            >
              <img class="my-5" :style="$vuetify.breakpoint.xs?'width:50px':'width:100px'" src="https://aungpyaenyein-21.github.io/anzu-dental-photos/treatments-icons/tooth-filling.png" alt="">
              <div
                class="treatment-name treatment1-name"
              >
                虫歯治療
              </div>
            </div>
          </v-col>
          <v-col
            cols="6"
            lg="4"
            md="4"
          >
            <div
              class="d-flex flex-column justify-start align-center"
            >
              <img class="my-5" :style="$vuetify.breakpoint.xs?'width:50px':'width:100px'" src="https://aungpyaenyein-21.github.io/anzu-dental-photos/treatments-icons/dental-cleaning.png" alt="">
                
              <div
                class="treatment-name treatment1-name"
              >
                歯周病治療
              </div>
            </div>
          </v-col>
          <v-col
            cols="6"
            lg="4"
            md="4"
          >
            <div
              class="d-flex flex-column justify-start align-center"
            >
              <img class="my-5" :style="$vuetify.breakpoint.xs?'width:50px':'width:100px'" src="https://aungpyaenyein-21.github.io/anzu-dental-photos/treatments-icons/tartar.png" alt="">
                
              <div
                class="treatment-name treatment1-name"
              >
                歯石除去
              </div>
            </div>
          </v-col>
          <v-col
            cols="6"
            lg="4"
            md="4"
          >
            <div
              class="d-flex flex-column justify-start align-center"
            >
              <img class="my-5" :style="$vuetify.breakpoint.xs?'width:50px':'width:100px'" src="https://aungpyaenyein-21.github.io/anzu-dental-photos/treatments-icons/bridge.png" alt="">
                
              <div
                class="treatment-name treatment1-name"
              >
                クラウン、ブリッジ<br>（被せ物の治療）
              </div>
            </div>
          </v-col>
          <v-col
            cols="6"
            lg="4"
            md="4"
          >
            <div
              class="d-flex flex-column justify-start align-center"
            >
              <img class="my-5" :style="$vuetify.breakpoint.xs?'width:50px':'width:100px'" src="https://aungpyaenyein-21.github.io/anzu-dental-photos/treatments-icons/root-canal.png" alt="">
              <div
                class="treatment-name treatment1-name d-flex flex-column justify-center align-center"
              >
                <span>根管治療</span>
                <span>（根の神経の治療）</span>
              </div>
            </div>
          </v-col>
          
          <v-col
            cols="6"
            lg="4"
            md="4"
          >
            <div
              class="d-flex flex-column justify-start align-center"
            >
              <img class="my-5" :style="$vuetify.breakpoint.xs?'width:50px':'width:100px'" src="https://aungpyaenyein-21.github.io/anzu-dental-photos/treatments-icons/dentures.png" alt="">
                
              <div
                class="treatment-name treatment1-name"
              >
                義歯（入れ歯）
              </div>
            </div>
          </v-col>
        </v-row>
        </div>
    </section>

    <!-- treatment2 -->
    <section
      class="treatments treatment2 d-flex flex-column justify-center align-center" 
      style="height:80vh;width:100vw;"
    >
      <div class="circle-container">
        <div class="circ2"
          :style="$vuetify.breakpoint.xs?'height:500px;width:500px;':'height:600px;width:600px;'"
        ></div>
      </div>
      <h1 
        class="my-5"
        :style="$vuetify.breakpoint.xs?'fontSize:2rem':'fontSize:3rem'"
      >自費治療</h1>
      <div
        :style="$vuetify.breakpoint.xs?'width:100vw':'width:50vw'"
      >
        <v-row>
          <v-col
            cols="6"
            lg="6"
            md="6"
          >
            <div
              class="d-flex flex-column justify-start align-center"
            >
              <img class="my-5" :style="$vuetify.breakpoint.xs?'width:50px':'width:100px'" src="https://aungpyaenyein-21.github.io/anzu-dental-photos/treatments-icons/whiting.png" alt="">
                
              <div
                class="treatment-name treatment2-name"
              >
              ホワイトニング
              </div>
            </div>
          </v-col>
          <v-col
            cols="6"
            lg="6"
            md="6"
          >
            <div
              class="d-flex flex-column justify-start align-center "
            >
              <img class="my-5" :style="$vuetify.breakpoint.xs?'width:50px':'width:100px'" src="https://aungpyaenyein-21.github.io/anzu-dental-photos/treatments-icons/dental-crown.png" alt="">
                
              <div
                class="treatment-name treatment2-name"
              >
                セラミック（白い被せ物など）
              </div>
            </div>
          </v-col>
        </v-row>
      </div>
      <p
        :style="$vuetify.breakpoint.xs?'width:80vw':'width:40vw'"
        class="text-center mt-10"
      >
        自費治療の費用については<br>その方に合う治療法を考えご提案致します。<br>ご相談ください。
      </p>
    </section>

    <!-- treatment3 -->
    <section
      class="treatments treatment3 d-flex flex-column justify-center align-center" 
      style="height:80vh;width:100vw;"
    >
      <div class="circle-container">
        <div class="circ3"
          :style="$vuetify.breakpoint.xs?'height:400px;width:400px;':'height:500px;width:500px;'"
        ></div>
      </div>
      <h1 
        class="my-5"
        :style="$vuetify.breakpoint.xs?'fontSize:2rem':'fontSize:3rem'"
      >矯正治療</h1>
      <div
        :style="$vuetify.breakpoint.xs?'width:100vw':'width:60vw'"
      >
        <v-row>
          <v-col
            cols="12"
          >
            <div
              class="d-flex flex-column justify-start align-center "
            >
              <img class="my-5" :style="$vuetify.breakpoint.xs?'width:50px':'width:100px'" src="https://aungpyaenyein-21.github.io/anzu-dental-photos/treatments-icons/orthodontic.png" alt="">
              <div
                class="treatment-name treatment3-name"
              >
                拡大床、ブラケット（ワイヤー矯正）、<br>アライナー矯正、インビザライン
              </div>
            </div>
          </v-col>
        </v-row>
      </div>
      <p
        :style="$vuetify.breakpoint.xs?'width:80vw':'width:60vw'"
        class="text-center mt-10"
      >
        矯正は月に一度、矯正科医が担当致します。
      </p>
    </section>  

    <!-- supplement -->
    <section
      style="height:100vh;width:100vw;"
      class="supplement d-flex flex-column justify-space-around align-center"
    >
      <h1 
        class="my-5"
        :style="$vuetify.breakpoint.xs?'fontSize:2rem':'fontSize:3rem'"
      > サプリメント</h1>
      <p>
        サプリメントのビタミンCは歯肉の出血を防ぐ効果もあり、内側からアプローチすることができます。
      </p>
      
    </section>

    <section
      class="about-clinic-text-warp  d-flex flex-column justify-center align-center"
      :style="$vuetify.breakpoint.xs?'height:50vh;width:100vw':'height:100vh;width:100vw;'"
    >
      <div 
        data-scroll="" 
        data-scroll-direction="horizontal" 
        data-scroll-speed="6" 
        class="about-clinic-text-outline"
        :style="$vuetify.breakpoint.xs?'fontSize:3rem;':'fontSize:12rem;'"
      >ABOUT CLINIC</div>
      <div 
        :style="$vuetify.breakpoint.xs?'fontSize:3rem;':'fontSize:12rem;'" 
        class="about-clinic-text"
      >ABOUT CLINIC</div>
      <div 
        data-scroll="" 
        data-scroll-direction="horizontal" 
        data-scroll-speed="-6"
        class="about-clinic-text-outline"
        :style="$vuetify.breakpoint.xs?'fontSize:3rem;':'fontSize:12rem;'" 
      >ABOUT CLINIC</div>
    </section>

    <section v-if="!$vuetify.breakpoint.xs" class="about-clinic">
      <div class="about-warp warp1 d-flex flex-column justify-center align-center">
        <h1>私たちの事</h1>
        <p class="mt-10" :style="$vuetify.breakpoint.xs?'width:80vw':'width:40vw'">
          ２０１４年７月に杏歯科医院はopenしました。治療が必要な方はもちろん、特に症状のない方でも気軽に足を運びたくなるようなクリニックを目指しています。
          <br>

          最近では、歯石を取るためなどで歯科のメインテナンスに通われている方が増えてきました。
          その方々が歯科医院に通われることになったのは、虫歯が出来たり、以前治療した歯の不具合だったりと、何らかの症状がきっかけで、という方が多いようです。
          歯周病は腫れや揺れなど患者さん自身で気づく症状が出る頃にはかなり状態が進んでいます。
          進行を止めることは出来ますが、状態が進むほど歯肉や歯槽骨を元通りに戻すことは難しくなる病気です。
          また、虫歯に関しても同様で、痛みが出る頃には状態が進んでいます。
          削って詰めたり、神経を取ってかぶせたりすることが出来ても、生まれもったエナメル質の美しさや神経のある状態には敵いません。
        </p>
      </div>
      <div class="about-warp warp2 d-flex justify-center align-center">
        <img 
          class="hover-image"
          height="60%" 
          src="https://aungpyaenyein-21.github.io/anzu-dental-photos/clinic-photos/entrance.jpg" 

        >
        <div class="entrance-title">Entrance</div>
        <div class="entrance-title outline">Entrance</div>
      </div>
      <div class="about-warp warp3">
        <img 
          class="hover-image consultation-image1"
          height="40%" 
          src="https://aungpyaenyein-21.github.io/anzu-dental-photos/clinic-photos/consultation.jpg" 
          alt=""
        >
        <img 
          class="hover-image consultation-image2"
          height="40%" 
          src="https://aungpyaenyein-21.github.io/anzu-dental-photos/clinic-photos/reception1.jpg" 
          alt=""
        >
        <img 
          class="hover-image consultation-image3"
          height="40%" 
          src="https://aungpyaenyein-21.github.io/anzu-dental-photos/clinic-photos/reception2.jpg" 
          alt=""
        >
        <div class="consultation-title">Consultation Room</div>
        <div class="outline-text">Consultation Room</div>
        <div class="consultation-paragraph">
          診療の前後の時間をゆったりと過ごしていただけるような空間にしました。
        </div>
        <!-- <div style="width:50%">
          <h1
            data-scroll="" data-scroll-direction="horizontal" data-scroll-delay="0.8"  data-scroll-speed="2"
          >これは consultation romm でございます。</h1>
          <h2
            data-scroll="" data-scroll-direction="horizontal" data-scroll-delay="0.8"  data-scroll-speed="2"
          >Lorem ipsum dolor sit amet, consectetur adipisicing elit. Totam, nobis. Quod illum placeat soluta officiis maiores veniam, repellendus enim ea, sed illo fuga eos. Corrupti voluptatibus laudantium illo dolorum earum?</h2>
        </div> -->
      </div>
      <div class="about-warp warp4">
        <img 
          class="sterilization-image"
          width="100%"
          src="https://aungpyaenyein-21.github.io/anzu-dental-photos/clinic-photos/sterilization-room.jpg" 
          alt=""
        >
        <div class="sterilization-text-warp pa-5">
          <div class="sterilization-text">Sterilization room</div>
          <div class="sterilization-paragraph">
            歯科医療には大切な器具、これらを消毒し、滅菌する為の消毒室は診療室と同じく非常に重要な場所です。来院された方からも見えるようオープンにし、スタッフにとっても意識をもって気持ちよく働ける場所としました。また、世界最高水準のクラスB規格の滅菌システムを導入しています。
            
          </div>
        </div>
      </div>
      <div class="warp5 d-flex justify-space-evenly align-center">
        
        <div
          class="d-flex  justify-center align-center treatment-images"
        >
          <img 
          class="treatment-image1"
            width="70%"
            src="https://aungpyaenyein-21.github.io/anzu-dental-photos/clinic-photos/treatment-room1.jpg" 
            alt=""
          >
        </div>
        <div class="treatment-text-warp pa-6" style="width:40%">
          <div class="treatment-text">Treatment Room</div>
          <div class="treatment-paragraph">
            根の先の病巣や、歯槽骨の形態、親知らずの位置などを把握するためにCTを導入しています。診療室には口腔外バキュームを設置しています。
          </div>
        </div>
        <div
          class="d-flex  justify-center align-center treatment-images"
        >
          <img 
          class="treatment-image2"
            width="70%"
            src="https://aungpyaenyein-21.github.io/anzu-dental-photos/clinic-photos/teatment-room2.jpg" 
            alt=""
          >
        </div>
      </div>
    </section>

    <!-- for mobile -->
    
    <section v-if="$vuetify.breakpoint.xs">
      <div class="mobile-warp1 d-flex flex-column justify-center align-center">
        <h1>私たちの事</h1>
        <p class="mt-10" :style="$vuetify.breakpoint.xs?'width:80vw':'width:40vw'">
          ２０１４年７月に杏歯科医院はopenしました。治療が必要な方はもちろん、特に症状のない方でも気軽に足を運びたくなるようなクリニックを目指しています。
          <br>

          最近では、歯石を取るためなどで歯科のメインテナンスに通われている方が増えてきました。
          その方々が歯科医院に通われることになったのは、虫歯が出来たり、以前治療した歯の不具合だったりと、何らかの症状がきっかけで、という方が多いようです。
          歯周病は腫れや揺れなど患者さん自身で気づく症状が出る頃にはかなり状態が進んでいます。
          進行を止めることは出来ますが、状態が進むほど歯肉や歯槽骨を元通りに戻すことは難しくなる病気です。
          また、虫歯に関しても同様で、痛みが出る頃には状態が進んでいます。
          削って詰めたり、神経を取ってかぶせたりすることが出来ても、生まれもったエナメル質の美しさや神経のある状態には敵いません。
        </p>
      </div>
      <div class="mobile-warp2 d-flex justify-center align-center">
        <img 
          data-scroll="" data-scroll-speed="2" 
          class="entrance-img"
          width="90%" 
          src="https://aungpyaenyein-21.github.io/anzu-dental-photos/clinic-photos/entrance.jpg" 
        >
        <div class="mobile-entrance-title">Entrance</div>
        <div class="mobile-entrance-title mobile-outline">Entrance</div>
      </div>
      <div class="mobile-warp3 d-flex justify-center align-center">
        <img 
          class="mobile-consultation-image1"
          width="70%" 
          src="https://aungpyaenyein-21.github.io/anzu-dental-photos/clinic-photos/consultation.jpg" 
          alt=""
          data-scroll="" data-scroll-speed="1" 
        >
        <img 
          class="mobile-consultation-image2"
          width="70%" 
          src="https://aungpyaenyein-21.github.io/anzu-dental-photos/clinic-photos/reception1.jpg" 
          alt=""
          data-scroll="" data-scroll-speed="2" 
        >
        <img 
          class="mobile-consultation-image3"
          width="70%" 
          src="https://aungpyaenyein-21.github.io/anzu-dental-photos/clinic-photos/reception2.jpg" 
          alt=""
          data-scroll="" data-scroll-speed="3" 
        >
        <div class="mobile-consultation-title">Consultation Room</div>
        <div class="mobile-outline-text">Consultation Room</div>
        <div class="mobile-consultation-paragraph">
          診療の前後の時間をゆったりと過ごしていただけるような空間にしました。
        </div>
      </div>
      <div
        class="mobile-warp4 d-flex flex-column justify-center align-center "
      >
        <img 
          data-scroll="" data-scroll-speed="2"
          width="90%"
          src="https://aungpyaenyein-21.github.io/anzu-dental-photos/clinic-photos/sterilization-room.jpg" 
          alt=""
        >
        <div class="mobile-sterilization-text">Sterilization room</div>
        <v-divider class="divider"></v-divider>
        <div class="mobile-sterilization-paragraph">
          歯科医療には大切な器具、これらを消毒し、滅菌する為の消毒室は診療室と同じく非常に重要な場所です。来院された方からも見えるようオープンにし、スタッフにとっても意識をもって気持ちよく働ける場所としました。また、世界最高水準のクラスB規格の滅菌システムを導入しています。
        </div>
      </div>
      <div
        class="mobile-warp5 d-flex flex-column justify-center align-center"
      >
        <img 
          width="80%"
          src="https://aungpyaenyein-21.github.io/anzu-dental-photos/clinic-photos/treatment-room1.jpg" 
          alt=""
          data-scroll="" data-scroll-speed="1" 
        >
        <img 
          width="80%"
          src="https://aungpyaenyein-21.github.io/anzu-dental-photos/clinic-photos/teatment-room2.jpg" 
          alt=""
          data-scroll="" data-scroll-speed="2" 
        >
        <div class="mobile-treatment-text">Treatment Room</div>
        <v-divider class="divider"></v-divider>
        <div class="mobile-treatment-paragraph">
          根の先の病巣や、歯槽骨の形態、親知らずの位置などを把握するためにCTを導入しています。診療室には口腔外バキュームを設置しています。
        </div>
      </div>
    </section>
    <section
      class="information-warp  d-flex flex-column justify-center align-center"
      :style="$vuetify.breakpoint.xs?'height:50vh;width:100vw':'height:100vh;width:100vw;'"
    >
      <div 
        data-scroll="" 
        data-scroll-direction="horizontal" 
        data-scroll-speed="6" 
        class="information-outline"
        :style="$vuetify.breakpoint.xs?'fontSize:3rem;':'fontSize:12rem;'"
      >CONTACT US</div>
      <div 
        :style="$vuetify.breakpoint.xs?'fontSize:3rem;':'fontSize:12rem;'" 
        class="information"
      >CONTACT US</div>
      <div 
        data-scroll="" 
        data-scroll-direction="horizontal" 
        data-scroll-speed="-6"
        class="information-outline"
        :style="$vuetify.breakpoint.xs?'fontSize:3rem;':'fontSize:12rem;'" 
      >CONTACT US</div>
    </section>
    <Footer/>
    <section 
      class="waiting"
    >
      <div class="waiting-text"
        :style="$vuetify.breakpoint.xs?'width:80%':''"
      >お待ちしております。</div>
      <div class="spin">
          <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 2300 1000">
              <title>Visit Site Link</title>
              <defs>
                  <path d="M50,250c0-110.5,89.5-200,200-200s200,89.5,200,200s-89.5,200-200,200S50,360.5,50,250" id="textcircle">
                      <animateTransform
                          attributeName="transform"
                          begin="0s"
                          dur="10s"
                          type="rotate"
                          from="0 250 250"
                          to="360 250 250"
                          repeatCount="indefinite" 
                          />
                  </path>
              </defs>
                  <text dy="70" textLength="1220">
                      <textPath xlink:href="#textcircle"> .Anzu.Dental.Clinic </textPath>
                  </text>
              </svg>
      </div>
    </section>
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
        scroller: null
      };
    },
    mounted(){
      this.setScroll();
      console.log('mounted')
    },
    beforeDestroy(){
      this.scroller.destroy()
      this.scroller = null
    },
    methods:{
      setScroll() {
        console.log('setscroll isrunning')
          this.scroller = new locomotiveScroll({
              el:  document.querySelector('.scroller'),
              smooth: true,
              smoothMobile: true
          });

          const scroller = this.scroller

          // this.x = scroller;
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
          // let Width = this.$vuetify.breakpoint.lg?'80%':'100%'
          // gsap.to('.day',{
          //     width:Width,
          //     scrollTrigger:{
          //         trigger:'.welcomeWarp',
          //         start:'center top',
          //         end:'80% top',
          //         scroller: ".scroller",
          //         // pin:true,
          //         markers:true,
          //         scrub:true,
          //     }
          // })
          gsap.from('.dental-lounge span',{
            y:'100px',opacity:0,stagger:.1,
            scrollTrigger:{
                trigger:'.second-warp',
                start:'center top',
                end:'bottom top',
                scroller: ".scroller",
                // pin:true,
                toggleActions: "restart none none none",
                markers:true,
                // scrub:true,
            }
          })
          gsap.from('.mission h1',{
            y:'100px',opacity:0,stagger:.1,
            scrollTrigger:{
                trigger:'.third-warp',
                start:'top top',
                end:'bottom top',
                scroller: ".scroller",
                // pin:true,
                toggleActions: "restart none none none",
                markers:true,
                // scrub:true,
            }
          })
          gsap.from('.treatment1 h1,.treatment1-name,.treatment1 img',{
            y:'100px',opacity:0,stagger:.1,
            scrollTrigger:{
                trigger:'.our-services',
                start:'center top',
                scroller: ".scroller",
                markers:true,
                toggleActions: "restart none none none",
            }
          })
          gsap.from('.treatment2 h1,.treatment2-name,.treatment2 img,.treatment2 p',{
            y:'100px',opacity:0,stagger:.1,
            scrollTrigger:{
                trigger:'.treatment1',
                start:'center top',
                scroller: ".scroller",
                markers:true,
                toggleActions: "restart none none none",
            }
          })
          gsap.from('.treatment3 h1,.treatment3-name,.treatment3 img,.treatment3 p',{
            y:'100px',opacity:0,stagger:.1,
            scrollTrigger:{
                trigger:'.treatment2',
                start:'center top',
                scroller: ".scroller",
                markers:true,
                toggleActions: "restart none none none",
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

          let pinWrap = document.querySelector(".about-clinic");
          let pinWrapWidth = pinWrap.offsetWidth;
          let horizontalScrollLength = pinWrapWidth - window.innerWidth;
          console.log({pinWrapWidth})
          console.log({horizontalScrollLength})
          gsap.to('.about-clinic',{
              x:-horizontalScrollLength,
              scrollTrigger:{
                  trigger:'.about-clinic',
                  start:'top top',
                  end: pinWrapWidth,
                  scroller: ".scroller",
                  pin:true,
                  markers:true,
                  scrub:true,

              }
          })
          gsap.from('.waiting-text',1,{
            opacity:0,
            scrollTrigger:{
              trigger:'.waiting',
              start:'-10px top',
              scroller: ".scroller",
              markers:true,
              toggleActions: "restart none none none",
            }
          })
          // gsap.to('.entrance-image',{
          //   height:'80%',
          //   filter:'none',
          //   scrollTrigger:{
          //     trigger:'.warp2',
          //     scroller: ".scroller",
          //     start:'center top',
          //     markers:true,
          //   }
          // })
          // gsap.to('.entrance-image',{
          //   height:'50%',
          //   filter:'none',
          //   scrollTrigger:{
          //     trigger:'.warp3',
          //     scroller: ".scroller",
          //     start:'center top',
          //     markers:true,
          //   }
          // })

          ScrollTrigger.addEventListener("refresh", () =>{
            // scroller.update()
            console.log({scroller})
            console.log('scroll trigger is update')
          }
          );
          scroller.update()
          ScrollTrigger.refresh();
      }
    }
  }
</script>

<style scoped>
  
  @import url('https://fonts.googleapis.com/css2?family=Noto+Sans+JP:wght@100;300;400;500;700;900&family=Noto+Serif+JP:wght@200;300;400;500;600;700;900&family=Playfair+Display:wght@600&family=Rampart+One&display=swap');
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

  /* html{
    margin: 0;
    padding: 0;
    overflow: hidden;
  } */

  .scroller{
    width: 100%;
    height: 100%;
    overflow: hidden;
    /* background-color: chartreuse; */
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
    /* background-color: #F8F7F5; */
    background: rgb(240,236,227);
    background: linear-gradient(0deg, #F5EEDC 0%, rgba(248,247,245,1) 100%);
  }
  .third-warp{
    widows: 100vw;
    background-color: #F5EEDC;
  }
  .mission{
    width: 100%;
  }
  .mission h1 {
    font-family: 'Noto Sans JP', sans-serif;
    font-weight: 500;
    letter-spacing: 1px;
  }
  .dental-lounge{
    width: 100%;
  }
  .dental-lounge span{
    margin: 0 10px 0 10px;
    color: #2B2B2B;
    /* color: rgb(85, 44, 33); */
    /* font-family: 'giaza'; */
    font-family: 'brightwall';
  }
  .bird{
    z-index: 3;
    position: absolute;
    top: -100px;
    left: -100px;
    transform: rotate(20deg);
  }
  .our-services{
    /* background: linear-gradient(0deg, #C2B49A 0%, #FAEED8 100%); */
    background-color: #87A7B3;
  }
  .service-outline{
    font-size: 10rem;
    -webkit-text-fill-color: transparent;
    -webkit-text-stroke-width: 1px;
    -webkit-text-stroke-color: #334A52;
    font-family: 'Rampart One', cursive;
    
    /* font-family: 'Alfa Slab One', cursive; */
  }
  .service{
    color: #334A52;
    font-family: 'Rampart One', cursive;
  }
  .about-clinic-text{
    font-family: 'Rampart One', cursive;
    color: #D9CAB3;
  }
  .about-clinic-text-outline{
    -webkit-text-fill-color: transparent;
    -webkit-text-stroke-width: 1px;
    -webkit-text-stroke-color: #D9CAB3;
    font-family: 'Rampart One', cursive;
  }
  .about-clinic-text-warp{
    background-color: #6D9886;
  }
  .information{
    font-family: 'Rampart One', cursive;
    color: #B89355;
  }
  .information-outline{
    -webkit-text-fill-color: transparent;
    -webkit-text-stroke-width: 1px;
    -webkit-text-stroke-color: #B89355;
    font-family: 'Rampart One', cursive;
  }
  .information-warp {
    background-color: #004736;
  }
  .treatment-name{
    font-family: 'Noto Sans JP', sans-serif;
    font-weight: 500;
    color: #EEEDDE;
    z-index: 10;
  }
  .treatments h1{
    /* font-family: 'Rampart One', cursive; */
    /* font-family: 'giaza'; */
    font-family: 'Noto Sans JP', sans-serif;
    font-weight: 900;
    color: #334A52;
    letter-spacing: 5px;
    /* font-size: 4rem; */
    z-index: 10;
  }
  .treatments img{
    z-index: 10;
  }
  .treatment1-names{
    letter-spacing: 10px;
    
  }
  .treatments{
    background-color: #87A7B3;
    
  }
  .treatment1{
    position: relative;
  }
  .treatment2{
    /* background-color: red; */
    position: relative;
  }
  .treatment2 p{
    font-family: 'Noto Sans JP', sans-serif;
    font-size: 1.5rem;
    font-weight: 700;
    color: #EEEDDE;
    z-index: 10;
  }
  .treatment3{
    position: relative;
  }
  .treatment3 p{
    font-family: 'Noto Sans JP', sans-serif;
    font-size: 1.5rem;
    font-weight: 700;
    color: #EEEDDE;
    z-index: 10;
  }
  .supplement{
    background-color: #87A7B3;
  }
  .supplement h1{
    font-family: 'Noto Sans JP', sans-serif;
    font-weight: 900;
    color: #334A52;
    letter-spacing: 5px;
    /* font-size: 4rem; */
    z-index: 10;
  }
  .supplement p {
    font-family: 'Noto Sans JP', sans-serif;
    font-size: 1.5rem;
    font-weight: 700;
    color: #EEEDDE;
    z-index: 10;
  }
  .about-clinic{
    width: 600vw;
    height: 100vh;
    /* background-color: white; */
    background-color: #6D9886;
    /* background-color:#FFF5EB; */
    display: flex;
    justify-content: start;
    overflow-y: hidden;
    /* position: absolute; */
  }
  .about-warp{
    height: 100vh;
    width: 100vw;
    position: relative;
  }
  .warp2{
    background-color:#FFF5EB;
    position: relative;
  }
  .mobile-warp2{
    background-color:#FFF5EB;
    height: 100vh;
    width: 100vw;
    position: relative;
  }

  .warp3{
    /* background-color: beige; */
    position: relative;
    /* background-color: #8FBDD3; */
  }
  .mobile-warp3{
    position: relative;
    background-color: #6D9886;
    width: 100vw;
    height: 100vh;
  }
  .warp4{
    /* background-color: cadetblue; */
  }
  .mobile-warp4{
    /* background-color: cadetblue; */
    background-color:#FFF5EB;
    height: 100vh;
    width: 100vw;
    position: relative;
  }
  .mobile-warp5{
    background-color: #6D9886;
    width: 100vw;
    height: 100vh;
  }
  .warp1{
    /* background-image: url("../assets/waiting.jpg");
    background-position: center;
    background-repeat: no-repeat; 
    background-size: cover;  */
  }
  .mobile-warp1{
    height: 100vh;
    width: 100vw;
    background-color: #6D9886;
  }
  .warp1 p{
    color: #F6F6F6;
    font-weight: 500;
    font-family: 'Noto Sans JP', sans-serif;
  }
  .mobile-warp1 p{
    color: #F6F6F6;
    font-weight: 500;
    font-family: 'Noto Sans JP', sans-serif;
  }
  .warp1 h1{
    color: #D9CAB3;;
    font-weight: 700;
    font-family: 'Noto Sans JP', sans-serif;
  }
  .mobile-warp1 h1{
    color: #D9CAB3;;
    font-weight: 700;
    font-family: 'Noto Sans JP', sans-serif;
  }
  .inner-warp{
    width: 80%;
    height: 80%;
    position: relative;
  }
  .entrance-text{
    position: absolute;
    bottom: 0;
    left: 0;
  }
  .entrance-text h1,.entrance-text h2{
    color: whitesmoke;
    
  }
  .hover-image{
    /* display: none; */
    /* transform: scale(0.7); */
    transition: all 1.5s;
    filter: grayscale(100%) sepia(20%) brightness(80%);
    z-index: 20;
  }
  .entrance-img{
    z-index: 20;
  }
  .hover-image:hover{
    filter: none;
    height: 77%;
    /* z-index: 3; */
  }

  .entrance-title{
    position: absolute;
    font-family: 'giaza';
    top: 95%;
    left: 10%;
    transform: translate(-10%,-95%);
    color: #DD4A48;
    /* font-family: 'giaza'; */
    font-size: 10rem;
    z-index: 5;
  }
  .mobile-entrance-title{
    position: absolute;
    font-family: 'giaza';
    top: 70%;
    left: 50%;
    transform: translate(-50%,-70%);
    color: #DD4A48;
    font-size: 5rem;
    z-index: 5;
  }

  .mobile-outline{
    /* color: black; */
    /* left: 20%; */
    -webkit-text-fill-color: transparent;
    -webkit-text-stroke-width: 1px;
    -webkit-text-stroke-color: #DD4A48;
    z-index: 30;
  }
  .outline{
    /* color: black; */
    /* left: 20%; */
    -webkit-text-fill-color: transparent;
    -webkit-text-stroke-width: 1px;
    -webkit-text-stroke-color: #DD4A48;
    z-index: 30;
  }

  .consultation-image1{
    position: absolute;
    top: 15%;
    left: 15%;
    transform: translate(-15%,-15%);
    z-index: 10;
  }
  .mobile-consultation-image1{
    position: absolute;
    top: 5%;
    left: 10px;
    transform: translate(10px,-5%);
    z-index: 10;
  }
  .consultation-image2{
    position: absolute;
    top: 15%;
    left: 85%;
    transform: translate(-85%,-15%);
    z-index: 10;
  }
  .mobile-consultation-image2{
    position: absolute;
    top: 30%;
    right: 10px;
    transform: translate(-10px);
    z-index: 10;
  }
  .consultation-image3{
    position: absolute;
    top: 90%;
    left: 15%;
    transform: translate(-15%,-90%);
    z-index: 10;
  }
  .mobile-consultation-image3{
    position: absolute;
    top: 50%;
    left: 10px;
    transform: translate(10px);
    z-index: 10;
  }
.consultation-title{
  position: absolute;
  font-family: 'giaza';
  top: 70%;
  left: 80%;
  transform: translate(-80%,-70%);
  color:#D9CAB3;
  font-size: 4rem;
  z-index: 0;
}
.mobile-consultation-title{
  position: absolute;
  font-family: 'giaza';
  top: 80%;
  left: 50%;
  transform: translate(-50%,-80%);
  color:#D9CAB3;
  font-size: 2rem;
  z-index: 0;
  width: 70%;
}
.consultation-paragraph{
  position: absolute;
  font-family: 'Noto Sans JP', sans-serif;
  top: 85%;
  left: 78%;
  transform: translate(-78%,-85%);
  z-index: 30;
  /* background-color: red; */
  color: white;
}
.mobile-consultation-paragraph{
  position: absolute;
  font-family: 'Noto Sans JP', sans-serif;
  top: 90%;
  left: 50%;
  transform: translate(-50%,-90%);
  z-index: 30;
  width: 70%;
  /* background-color: red; */
  color: white;
}

.outline-text{
  position: absolute;
  font-family: 'giaza';
  top: 70%;
  left: 80%;
  transform: translate(-80%,-70%);
  font-size: 4rem;
  z-index: 30;
  -webkit-text-fill-color: transparent;
  -webkit-text-stroke-width: 1px;
  -webkit-text-stroke-color:#D9CAB3;
}
.mobile-outline-text{
  position: absolute;
  font-family: 'giaza';
  top: 80%;
  left: 50%;
  transform: translate(-50%,-80%);
  font-size: 2rem;
  z-index: 30;
  -webkit-text-fill-color: transparent;
  -webkit-text-stroke-width: 1px;
  -webkit-text-stroke-color:#D9CAB3;
  width: 70%;
}
.warp4{
  position: relative;
}

.sterilization-image{
  /* position: absolute;
  top: 15%;
  left: 90%;
  transform: translate(-90%,-15%); */
  transition: all 1.5s;
  filter: grayscale(100%) sepia(20%) brightness(80%);
  transform: scale(1.05);
}
.sterilization-image:hover{
  filter: none;
  transform: scale(1);
  /* height: 0%; */
}
.sterilization-text-warp{
  position: absolute;
  top: 45%;
  left: 50%;
  transform: translate(-50%,-45%);
  background-color: #6D9886;
}
.sterilization-text{

  color:#D9CAB3;
  font-size: 5rem;
  font-family: 'giaza';
  transition: all 1.5s;
}
.mobile-sterilization-text{
  color: #DD4A48;
  font-size: 2.5rem;
  font-family: 'giaza';
  z-index: 20;
}
.sterilization-text:hover{
  -webkit-text-fill-color: transparent;
  -webkit-text-stroke-width: 1px;
  -webkit-text-stroke-color: #D9CAB3;
}
.sterilization-paragraph{
  font-family: 'Noto Sans JP', sans-serif;
  color: white;
}
.mobile-sterilization-paragraph{
  font-family: 'Noto Sans JP', sans-serif;
  color: gray;
  width: 80%;
}
.divider{
  width: 60%;
  margin-bottom: 2rem;
  margin-top: 1rem;
}
.warp5{
  /* background-color:#2B2B2B; */
  height: 100vh;
  width: 200vw;
  /* background-color: aqua; */
}
.treatment-text-warp{
  /* background-color: red; */
}
.treatment-text{
  color: #D9CAB3;
  font-size: 4rem;
  font-family: 'giaza';
  /* -webkit-text-fill-color: transparent;
  -webkit-text-stroke-width: 1px;
  -webkit-text-stroke-color: #D9CAB3; */
}
.mobile-treatment-text{
  color: #D9CAB3;
  font-size: 3rem;
  font-family: 'giaza';
  z-index: 10;
}

.treatment-paragraph{
  font-family: 'Noto Sans JP', sans-serif;
  color: white;
}
.mobile-treatment-paragraph{
  font-family: 'Noto Sans JP', sans-serif;
  color: white;
  width: 80%;
}
.treatment-images{
  height: 100%;
  /* background-color: #2B2B2B; */
  /* background-color:#FFF5EB; */
}
.treatment-image1{
  transition: all 1.5s;
  filter: grayscale(100%) sepia(20%) brightness(80%);
}
.treatment-image1:hover{
  filter: none;
  width: 90%;
}
.warp6{
  /* background-color: #2B2B2B; */
  /* background-color:#FFF5EB; */
}
.treatment-image2{
  transition: all 1.5s;
  filter: grayscale(100%) sepia(20%) brightness(80%);
}
.treatment-image2:hover{
  filter: none;
  width: 90%;
}
.waiting{
  height: 100vh;
  width: 100vw;
  background-image: url("https://aungpyaenyein-21.github.io/anzu-dental-photos/clinic-photos/waiting.jpg"); /* The image used */
  background-position: center; /* Center the image */
  background-repeat: no-repeat; /* Do not repeat the image */
  background-size: cover; /* Resize the background image to cover the entire container */
  position: relative;
}
.waiting-text{
  position: absolute;
  left: 50%;
  top: 30%;
  transform: translate(-50%,-30%);
  font-size: 2rem;
  font-family: 'Noto Serif JP', serif;
  color: rgb(85, 44, 33);
  font-weight: 500;
}
  .spin{
      position: absolute;
      top: -9%;
      left: 50%;
      transform: translate(-50%,-9%);
      width: 200px;
  }
  svg { width: 500%; }
  svg textPath { 
  font-size: 63px;
      font-family: 'giaza';
      text-transform: uppercase;
      letter-spacing: 20px;
      fill: #B89355;
  background: #B89355;
  }
  @keyframes spin{
  100%{
      transform: rotate(360deg);
  }
  }
  .circ1{
  /* border: 1px solid rgb(85, 44, 33); */
  border-radius: 92% 110% 132% 88%;
  /* position: absolute;
  left: 0;
  top: 0; */
  animation: spin 6s linear infinite;
  /* background-color: thistle; */
  background-color: #7995a0;
  }
  .circ2{
  border-radius: 132% 88% 92% 110%;
  animation: spin 3s linear infinite;
  background-color: #7995a0;
  }
  .circ3{
  border-radius: 92% 110% 132% 88%;
  animation: spin 4s linear infinite;
  background-color: #7995a0;
  }

  /* .circ:nth-of-type(1){
  animation-duration: 3s;
  border-radius: 132% 88% 92% 110%;
  }


  .circ:nth-of-type(2){
  animation-duration: 8s;
  border-radius: 75% 122% 60% 160%;
  } */

  .circle-container{
  position: relative;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%,-50%);
  z-index: 5;
  }
</style>
