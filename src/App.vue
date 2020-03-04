<template>
  <v-app id="main">
    <v-card>
      <v-card-title class="header">
        <div class="wrap-image">
          <div class="wrap-inside" :style="{'background-image': 'url(/img/foto_p1.jpeg)'}"></div>
        </div>
        <div class="wrap-text">
          <h1 class="name">Abdul Muhit T.</h1>
          <p class="title">Web developer</p>
        </div>

        <div class="medsos">
          <div class="meditem" :style="{'background-image': 'url(/img/icons/icon_loc.svg)'}"></div>
          <div class="meditem" :style="{'background-image': 'url(/img/icons/icon_loc.svg)'}"></div>
          <div class="meditem" :style="{'background-image': 'url(/img/icons/icon_loc.svg)'}"></div>
          <div class="meditem" :style="{'background-image': 'url(/img/icons/icon_loc.svg)'}"></div>
          <div class="meditem" :style="{'background-image': 'url(/img/icons/icon_loc.svg)'}"></div>
          <div class="meditem" :style="{'background-image': 'url(/img/icons/icon_loc.svg)'}"></div>
        </div>

        <div class="email">
          <div class="medemail" :style="{'background-image': 'url(/img/icons/icon_loc.svg)'}"></div>
          <div class="medemail" :style="{'background-image': 'url(/img/icons/icon_loc.svg)'}"></div>
        </div>
      </v-card-title>
      <v-tabs v-model="tab" background-color="transparent" grow>
        <v-tab v-for="item in items" :key="item">{{ item }}</v-tab>
      </v-tabs>
      <v-tabs-items v-model="tab">
        <!--    <v-tab-item v-for="item in items" :key="item">
          <v-card flat>
            <v-card-text>{{ text }}</v-card-text>
          </v-card>
        </v-tab-item>-->

        <v-tab-item>
          <v-card flat>
            <v-card-text>Satu</v-card-text>
          </v-card>
        </v-tab-item>

        <v-tab-item>
          <v-card flat>
            <v-card-text>dua</v-card-text>
          </v-card>
        </v-tab-item>

        <v-tab-item>
          <v-card flat>
            <v-card-text>tiga</v-card-text>
          </v-card>
        </v-tab-item>

        <v-tab-item>
          <v-card flat>
            <v-card-text>empat</v-card-text>
          </v-card>
        </v-tab-item>

        <v-tab-item>
          <v-card flat>
            <v-card-text>lima</v-card-text>
          </v-card>
        </v-tab-item>

        <v-tab-item>
          <v-card flat>
            <v-card-text>Satu</v-card-text>
          </v-card>
        </v-tab-item>
      </v-tabs-items>
    </v-card>
  </v-app>
</template>
<script>
export default {
  name: "App",
  data: () => ({
    tab: null,
    items: ["About", "PortFolio", "Work", "Education", "Skills"],
    text:
      "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat."
  })
};
</script>

<style lang="scss">
* {
  font-family: "Open Sans", sans-serif;
}

.header {
  display: flex;
  justify-content: flex-start;
  align-items: center;
  background: #1d1d1d;
  box-shadow: 0px 6px 30px rgba(0, 0, 0, 0.12);

  .wrap-image {
    .wrap-inside {
      display: block;
      width: 85px;
      height: 85px;
      background-color: #edeff2;
      border-radius: 50%;
      background-repeat: no-repeat;
      background-position: center center;
      background-size: cover;

      /*   img {
        border-radius: 50%;
      } */
    }
  }

  .wrap-text {
    .name {
      font-weight: 600;
      font-size: 22px;
      line-height: 30px;
      color: #ffffff;
    }

    .title {
      font-size: 12px !important;
      line-height: 16px;
      color: #ffffff;
    }
  }

  .medsos {
    display: grid;
    grid-template: 20px 20px / repeat(6, 23%);
    text-align: center;
    margin-top: 37px;

    .meditem {
      display: block;
      width: 37px;
      height: 37px;
      background-color: #edeff2;
      border-radius: 50%;
      background-position: center center;
      background-size: cover;
      margin-right: 5px;
    }
  }

  .email {
    display: flex;
    flex-basis: 100%;
    margin-top: 37px;
    justify-content: center;

    .medemail {
      display: block;
      width: 52px;
      height: 52px;
      background-color: #edeff2;
      border-radius: 50%;
      background-position: center center;
      background-size: cover;
      margin-right: 10px;
    }
  }
}

.header > div {
  margin-right: 10px;
}
</style>
