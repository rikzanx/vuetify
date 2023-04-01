<template>
  <v-toolbar app class="bg-white">
    <span class="hidden-sm-and-up">
      <v-toolbar-side-icon @click="sidebar = !sidebar">
      </v-toolbar-side-icon>
    </span>
    <v-toolbar-title>

      <router-link to="/" tag="span" style="cursor: pointer">
        <v-img height="50" src="@/assets/logo-1.png" />
      </router-link>

    </v-toolbar-title>
    <v-spacer></v-spacer>

    <v-toolbar-items class="hidden-xs-only">
      <!-- <div class="coba">
         <v-text-field class="pencarian" v-model="firstName" :rules="rules" bg-color="white">

          </v-text-field>
          <v-btn type="submit" inline-block class="mt-2"></v-btn>
      </div> -->

      <v-row
        align="center"
        no-gutters
        style="height:80px; background-color:blue;"
      >
        <v-col
        >
          <v-text-field class="pencarian" v-model="firstName" :rules="rules" bg-color="white">

            </v-text-field>
        </v-col>
</v-row>






      <v-menu>
        <template v-slot:activator="{ props }">
          <v-btn v-bind="props" variant="text">
            Singapore
            <v-icon right dark>mdi-menu-down</v-icon>
          </v-btn>
        </template>
        <v-list>
          <v-list-item v-for="(item, index) in items" :key="index" :value="index">
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item>
        </v-list>
      </v-menu>
      <v-btn href='/home' variant="outlined" style="background-color: #0596D5;color:white;">
        Sign Up/Register
      </v-btn>
      <v-menu>
        <template v-slot:activator="{ props }">
          <v-img height="50" src="@/assets/logo-1.png" />
          <v-btn icon="mdi-menu" v-bind="props"></v-btn>
        </template>

        <v-list>
          <v-list-item v-for="(item, i) in items" :key="i">
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item>
        </v-list>
      </v-menu>
    </v-toolbar-items>
  </v-toolbar>

    <v-container>
    <v-row>
      <v-col cols="12">
        <div class="d-flex justify-space-between" style="background-color:red;">
      <router-link to="/" tag="span" style="cursor: pointer">
        <v-img height="50" width="50px" src="@/assets/logo-1.png" />
      </router-link>

      <div class="div" style="width:350px;height:50px;background-color:white;">
        <v-text-field append-inner-icon="mdi-magnify" single-line></v-text-field>
        <!-- <v-img height="50" width="50px" src="@/assets/logo-1.png" />
         -->
      </div>

      <router-link to="/" tag="span" style="cursor: pointer">
        <v-img height="50" width="50px" src="@/assets/logo-1.png" />
      </router-link>

      <router-link to="/" tag="span" style="cursor: pointer">
        <v-img height="50" width="150px" src="@/assets/logo-1.png" />
      </router-link>

      <router-link to="/" tag="span" style="cursor: pointer">
        <v-img height="50" width="150px" src="@/assets/logo-1.png" />
      </router-link>

      <router-link to="/" tag="span" style="cursor: pointer">
        <v-img height="50" width="100px" src="@/assets/logo-1.png" />
      </router-link>
        </div>
      </v-col>
    </v-row>
  </v-container>


  <v-sheet class="d-flex align-center justify-center flex-wrap text-center mx-auto" elevation="0" min-height="600"
    width="100%">
    <v-img width="100%" src="@/assets/header.png" />
    <div class="jumbotron-text">

      <p align="center" class="header-title">What are you Looking for.. ?</p>
      <p class="header-title-sub">The gypsy Trending Web Apps</p>
    </div>
  </v-sheet>




  <v-container>
    <v-row>
      <v-col cols="6" offset="3">
        <div class="d-flex flex-row justify-center mb-6 ">
          <v-btn class="sub-menu-btn active">
            View All
            <span class="badge active">2.7K</span>
          </v-btn>
          <v-btn class="sub-menu-btn">
            Illustration
            <span class="badge">2.7K</span>
          </v-btn>
          <v-btn class="sub-menu-btn">
            Branding
            <span class="badge">2.7K</span>
          </v-btn>
          <v-btn class="sub-menu-btn">
            Product Design
            <span class="badge">2.7K</span>
          </v-btn>
          <v-btn class="sub-menu-btn">
            Typography
            <span class="badge">2.7K</span>
          </v-btn>
        </div>
      </v-col>
    </v-row>

    <v-row>
      <v-col cols="4">
        <v-card>
          <v-img src="@/assets/gypsi-1.png" class="align-end" gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
            height="200px" cover></v-img>
          <v-card-title class="text-black">Mall-e</v-card-title>
          <v-card-subtitle>
            1,000 miles of wonder
          </v-card-subtitle>
          <v-card-actions>
            <v-btn elevation="4">
              Explore
            </v-btn>
            <v-spacer></v-spacer>
            <span>
              <v-icon>mdi-eye</v-icon>
              1336
            </span>
          </v-card-actions>
        </v-card>
      </v-col>
      <v-col cols="4">
        <v-card>
          <v-img src="@/assets/gypsi-1.png" class="align-end" gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
            height="200px" cover></v-img>
          <v-card-title class="text-black">Mall-e</v-card-title>
          <v-card-subtitle>
            1,000 miles of wonder
          </v-card-subtitle>
          <v-card-actions>
            <v-btn elevation="4">
              View App
            </v-btn>
            <v-spacer></v-spacer>
            <span>
              <v-icon>mdi-eye</v-icon>
              1336
            </span>
          </v-card-actions>
        </v-card>
      </v-col>
      <v-col cols="4">
        <v-card>
          <v-img src="@/assets/gypsi-1.png" class="align-end" gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
            height="200px" cover></v-img>
          <v-card-title class="text-black">Mall-e</v-card-title>
          <v-card-subtitle>
            1,000 miles of wonder
          </v-card-subtitle>
          <v-card-actions>
            <v-btn elevation="4">
              Explore
            </v-btn>
            <v-spacer></v-spacer>
            <span>
              <v-icon>mdi-eye</v-icon>
              1336
            </span>
          </v-card-actions>
        </v-card>
      </v-col>
      <v-col cols="4">
        <v-card>
          <v-img src="@/assets/gypsi-1.png" class="align-end" gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
            height="200px" cover></v-img>
          <v-card-title class="text-black">Mall-e</v-card-title>
          <v-card-subtitle>
            1,000 miles of wonder
          </v-card-subtitle>
          <v-card-actions>
            <v-btn elevation="4">
              Explore
            </v-btn>
            <v-spacer></v-spacer>
            <span>
              <v-icon>mdi-eye</v-icon>
              1336
            </span>
          </v-card-actions>
        </v-card>
      </v-col>
      <v-col cols="4">
        <v-card>
          <v-img src="@/assets/gypsi-1.png" class="align-end" gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
            height="200px" cover></v-img>
          <v-card-title class="text-black">Mall-e</v-card-title>
          <v-card-subtitle>
            1,000 miles of wonder
          </v-card-subtitle>
          <v-card-actions>
            <v-btn elevation="4">
              Explore
            </v-btn>
            <v-spacer></v-spacer>
            <span>
              <v-icon>mdi-eye</v-icon>
              1336
            </span>
          </v-card-actions>
        </v-card>
      </v-col>
      <v-col cols="4">
        <v-card>
          <v-img src="@/assets/gypsi-1.png" class="align-end" gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
            height="200px" cover></v-img>
          <v-card-title class="text-black">Mall-e</v-card-title>
          <v-card-subtitle>
            1,000 miles of wonder
          </v-card-subtitle>
          <v-card-actions>
            <v-btn elevation="4">
              Explore
            </v-btn>
            <v-spacer></v-spacer>
            <span>
              <v-icon>mdi-eye</v-icon>
              1336
            </span>
          </v-card-actions>
        </v-card>
      </v-col>
      <v-col cols="4">
        <v-card>
          <v-img src="@/assets/gypsi-1.png" class="align-end" gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
            height="200px" cover></v-img>
          <v-card-title class="text-black">Mall-e</v-card-title>
          <v-card-subtitle>
            1,000 miles of wonder
          </v-card-subtitle>
          <v-card-actions>
            <v-btn elevation="4">
              Explore
            </v-btn>
            <v-spacer></v-spacer>
            <span>
              <v-icon>mdi-eye</v-icon>
              1336
            </span>
          </v-card-actions>
        </v-card>
      </v-col>
      <v-col cols="4">
        <v-card>
          <v-img src="@/assets/gypsi-1.png" class="align-end" gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
            height="200px" cover></v-img>
          <v-card-title class="text-black">Mall-e</v-card-title>
          <v-card-subtitle>
            1,000 miles of wonder
          </v-card-subtitle>
          <v-card-actions>
            <v-btn elevation="4">
              Explore
            </v-btn>
            <v-spacer></v-spacer>
            <span>
              <v-icon>mdi-eye</v-icon>
              1336
            </span>
          </v-card-actions>
        </v-card>
      </v-col>
      <v-col cols="4">
        <v-card>
          <v-img src="@/assets/gypsi-1.png" class="align-end" gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
            height="200px" cover></v-img>
          <v-card-title class="text-black">Mall-e</v-card-title>
          <v-card-subtitle>
            1,000 miles of wonder
          </v-card-subtitle>
          <v-card-actions>
            <v-btn elevation="4">
              Explore
            </v-btn>
            <v-spacer></v-spacer>
            <span>
              <v-icon>mdi-eye</v-icon>
              1336
            </span>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
  </v-container>

  <v-container class="mb-6">
    <v-row>
      <v-col cols="12">
        <p align="center" class="header-title">Become Our Partner</p>
        <p class="header-title-sub">As a Rider , Merchant , Employer , Agency</p>
      </v-col>
    </v-row>
    <v-row>
      <v-col cols="4">
        <v-card>
          <v-img src="@/assets/partner-1.png" class="align-end" gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
            height="200px" cover></v-img>
          <v-card-title class="text-black text-center">As a Rirder/Driver</v-card-title>
          <v-card-text class="text-center">
            Earn money by delivering food from restaurant. All you need are the skills and a bike
          </v-card-text>
          <v-card-actions align="center">
            <v-btn elevation="0" class="mx-auto bg-info">
              Explore
            </v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
      <v-col cols="4">
        <v-card>
          <v-img src="@/assets/partner-1.png" class="align-end" gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
            height="200px" cover></v-img>
          <v-card-title class="text-black text-center">As a Rirder/Driver</v-card-title>
          <v-card-text class="text-center">
            Earn money by delivering food from restaurant. All you need are the skills and a bike
          </v-card-text>
          <v-card-actions align="center">
            <v-btn elevation="0" class="mx-auto bg-info">
              Explore
            </v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
      <v-col cols="4">
        <v-card>
          <v-img src="@/assets/partner-1.png" class="align-end" gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
            height="200px" cover></v-img>
          <v-card-title class="text-black text-center">As a Rirder/Driver</v-card-title>
          <v-card-text class="text-center">
            Earn money by delivering food from restaurant. All you need are the skills and a bike
          </v-card-text>
          <v-card-actions align="center">
            <v-btn elevation="0" class="mx-auto bg-info">
              Explore
            </v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
  <hr>
  <v-container class="mt-6">
    <v-row>
      <v-col cols="12">
        <div class="d-flex flex-row justify-center mb-6 ">
          <div class="about">
            <h2>About the gypsum</h2>
            <hr width="25%">
            <p>The gypsy is a Super App that is useful for users travelling from point A to point B in search of anything
              and everything!!!</p>
            <p>
              <a>
                <v-icon color="blue">mdi-menu</v-icon> Marine drive, Singapore
              </a>
            </p>
            <p>
              <a>
                <v-icon color="blue">mdi-menu</v-icon> Marine drive, Singapore
              </a>
            </p>
            <p>
              <a>
                <v-icon color="blue">mdi-menu</v-icon> Marine drive, Singapore
              </a>
            </p>
            <p>
              <a>
                <v-icon color="blue">mdi-menu</v-icon> Marine drive, Singapore
              </a>
            </p>

          </div>
          <div class="about">
            <h2>About the gypsum</h2>
            <hr width="25%">
            <p>The gypsy is a Super App that is useful for users travelling from point A to point B in search of anything
              and everything!!!</p>
            <p>
              <a>
                <v-icon color="blue">mdi-menu</v-icon> Marine drive, Singapore
              </a>
            </p>
            <p>
              <a>
                <v-icon color="blue">mdi-menu</v-icon> Marine drive, Singapore
              </a>
            </p>
            <p>
              <a>
                <v-icon color="blue">mdi-menu</v-icon> Marine drive, Singapore
              </a>
            </p>
            <p>
              <a>
                <v-icon color="blue">mdi-menu</v-icon> Marine drive, Singapore
              </a>
            </p>

          </div>
          <div class="about">
            <h2>About the gypsum</h2>
            <hr width="25%">
            <p>The gypsy is a Super App that is useful for users travelling from point A to point B in search of anything
              and everything!!!</p>
            <p>
              <a>
                <v-icon color="blue">mdi-menu</v-icon> Marine drive, Singapore
              </a>
            </p>
            <p>
              <a>
                <v-icon color="blue">mdi-menu</v-icon> Marine drive, Singapore
              </a>
            </p>
            <p>
              <a>
                <v-icon color="blue">mdi-menu</v-icon> Marine drive, Singapore
              </a>
            </p>
            <p>
              <a>
                <v-icon color="blue">mdi-menu</v-icon> Marine drive, Singapore
              </a>
            </p>

          </div>
          <div class="about">
            <h2>About the gypsum</h2>
            <hr width="25%">
            <p>The gypsy is a Super App that is useful for users travelling from point A to point B in search of anything
              and everything!!!</p>
            <p>
              <a>
                <v-icon color="blue">mdi-menu</v-icon> Marine drive, Singapore
              </a>
            </p>
            <p>
              <a>
                <v-icon color="blue">mdi-menu</v-icon> Marine drive, Singapore
              </a>
            </p>
            <p>
              <a>
                <v-icon color="blue">mdi-menu</v-icon> Marine drive, Singapore
              </a>
            </p>
            <p>
              <a>
                <v-icon color="blue">mdi-menu</v-icon> Marine drive, Singapore
              </a>
            </p>

          </div>

        </div>

      </v-col>
    </v-row>
  </v-container>

  <v-footer class="bg-black text-center d-flex flex-column">
    <div class="pt-0">
      @ The gypsy International | Singapore, India 2023 - 2025
      <v-btn variant="text" icon="mdi-home"></v-btn>
      <v-btn variant="text" icon="mdi-home"></v-btn>
      <v-btn variant="text" icon="mdi-home"></v-btn>
      <v-btn variant="text" icon="mdi-home"></v-btn>
    </div>
  </v-footer>


<v-row
        align="center"
        no-gutters
        style="height: 150px; background-color:blue;"
      >
        <v-col
        >
          <v-text-field class="pencarian" v-model="firstName" :rules="rules" bg-color="white">

            </v-text-field>
        </v-col>
</v-row>
    <!-- <div class="nyobak" align="center" style="height:600px;background-color:blue;">
      <v-text-field class="pencarian" v-model="firstName" :rules="rules" bg-color="white">

            </v-text-field>
    </div> -->


</template>

<script setup>
</script>

<script>
//import HelloWorld from "./components/HelloWorld";

export default {
  name: "App",
  data() {
    return {
      appTitle: 'Awesome App',
      sidebar: false,
      menuItems: [
        { title: 'Home', path: '/home', icon: 'home' },
        { title: 'Sign Up', path: '/signup', icon: 'face' },
        { title: 'Sign In', path: '/signin', icon: 'lock_open' }
      ],
      items: [
        { title: 'Home', path: '/home', icon: 'home' },
        { title: 'Sign Up', path: '/signup', icon: 'face' },
        { title: 'Sign In', path: '/signin', icon: 'lock_open' }
      ]
    }
  },
};
</script>

<style>
.v-text-field,.v-input__control{
  height: 50px !important;
}

:deep(.pencarian){
  border-block-color: red;
}
.input-area {
  width: 300px;
  border-top: 1px solid black;
  border-bottom: 1px solid black;
  border-left: 5px solid red;
  height: 42px;
  display: inline-block;
}

.button-search {
  display: inline-block;
  height: 43px !important;
  width: 42px !important;
  background-color: red;
}

.coba {

}


.sub-menu-btn {
  border-radius: 50px !important;
  color: black !important;
  margin: 2px;
}

.sub-menu-btn.active {
  background: #C2D5E9 !important;
  border-radius: 50px !important;
  color: black !important;
  padding: 6px 10px !important;
  margin: 2px;
}

.badge {
  border-radius: 50px;
  background: #D9D9D9;
  color: black;
  padding: 5px;
}

.badge.active {
  border-radius: 50px;
  background: #0596D5;
  color: white;
  padding: 5px;
}

.jumbotron-text {
  padding-top: 50px;
  padding-bottom: 50px;
}

.header-title {
  color: black;
  font-family: 'Nunito';
  font-style: normal;
  font-weight: 700;
  font-size: 56px;
  line-height: 76px;
}

.header-title-sub {
  text-align: center;
  font-family: 'Nunito';
  font-style: normal;
  font-weight: 700;
  font-size: 32px;
  line-height: 44px;
  color: #808080;
}
</style>
