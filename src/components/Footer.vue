<template>
    <div id="app">
  
    <v-footer
      dark
      padless
    >
      <v-card
        class="flex"
        flat
        tile
      >
        <v-card-title class="teal">
          <h5>Far Out Himalayas</h5>
           <h5>1235 University Boulevard</h5>
           <h5>Steubenville, Ohio</h5>
           <h5>43952</h5>
           <h5>(740)283-3771</h5>
          <v-spacer></v-spacer>
  
          <v-btn 
            v-for="icon in icons"
            :key="icon"
            class="mx-4 text-center"
            dark
            icon
          >
            <v-icon size="24px">{{ icon }}</v-icon>
          </v-btn>
        </v-card-title>
  
        <v-card-text class="py-2 white--text text-center">
          {{ new Date().getFullYear() }} — <strong>Bulid by Mohit</strong>
        </v-card-text>
      </v-card>
    </v-footer>
  
</div>
</template>
<script>
export default {
   name: 'app',
  data: () => ({
    icons: [
         'mdi-facebook',
      'mdi-twitter',
      'mdi-linkedin',
      'mdi-instagram',
    ],
  }),

    
   
}
</script>