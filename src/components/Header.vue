<template>
  <v-app>
    <v-app-bar app color="white">
      <div class="d-flex align-center">
        <router-link to="/">
          <v-img
            alt="Far Out Himalayas Logo"
            class="shrink mr-2"
            contain
            src="https://farout.herokuapp.com/static/FOH.PNG"
            transition="scale-transition"
            width="40"
          />
        </router-link>

        <v-app-title class="headline text-uppercase">
          <span class="font-weight-light red--text">Far Out Himalayas</span>
        </v-app-title>
      </div>

      <v-spacer></v-spacer>

      <router-link to="/about">
        <v-btn>
          <span class="mr-2">ABOUT US</span>
        </v-btn>
      </router-link>
      <router-link to="/login">
        <v-btn>
          <span class="mr-2">Login</span>
        </v-btn>
      </router-link>
      <router-link to="/sign up">
        <v-btn>
          <span class="mr-2">SIGN UP</span>
        </v-btn>
      </router-link>
    </v-app-bar>
  </v-app>
</template>

<script>
export default {
  name: "Header",
  props: {
    title: String,
  },
  data: function () {
    return {
      name: "Mohit",
    };
  },
};
</script>




