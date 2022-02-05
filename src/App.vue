<template>
  <v-app style="position: relative;">
    <div class="main-logo">
      <v-img
        src="	http://dentallounge.jp/site_anzu/wp-content/themes/anzu/images/logo.png"
        width="300"
      />
    </div>

    <div class="menu">
      <v-dialog
        v-model="menuDialog"
        fullscreen
        transition="dialog-bottom-transition"
      >
        <template v-slot:activator="{ on, attrs }">
          <v-btn
            icon
            v-bind="attrs"
            v-on="on"
            x-large
          >
            <v-icon>mdi-menu</v-icon>
          </v-btn>
        </template>
        <v-card>
          <p @click="menuDialog = false">hello</p>
        </v-card>
      </v-dialog>
    </div>
    

    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script>

export default {
  name: 'App',

  data: () => ({
    menuDialog:false,
  }),
};
</script>

<style scoped>
.main-logo{
  position: absolute;
  top: 10px;
  left: 10px;
  /* transform: translate(-10px,-10px); */
}
.menu{
  position: absolute;
  top: 10px;
  right: 10px;
  z-index: 1;
}
.close-menu{
  position: absolute;
  top: 10px;
  right: 10px;
  z-index: 1;
}
</style>
