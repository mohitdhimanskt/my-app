<template>
    
    <v-app class=" text-center mg-4">
      

      <v-app-title class="d-lg-flex mb-4">
         
           <v-carousel
      cycle
      height="400"
      hide-delimiter-background
      show-arrows-on-hover
    >
      <v-carousel-item
         v-for="(item,i) in items"
        :key="i"
        :src="item.src"
        reverse-transition="fade-transition"
        transition="fade-transition"
      >
       
                  
          
        <h1 class="display-2 text-center font-weight-bold white--text mb-16">
          Experience The Best of Himalayas<br>
          We provide Best Guidance
          Your travel partner in Himalayas
        </h1>
        

        <p class="subheading font-weight-regular white--text">
          Praesent sit amet fermentum ipsum. Cras dictum ante nec metus pretium, <br>
      placerat hendrerit ex facilisis. Ut sed neque sem. Ut ipsum dolor, dapibus et<br>
                 imperdiet nec, ultricies non metus.</p>
          </v-carousel-item>
    </v-carousel>
      </v-app-title>
    </v-app>
    
</template>
<script>
export default {
  name: "Heroslider",
  data () {
    return {
      items: [
        {
          src: 'https://www.wellnessonfire.com/wp-content/uploads/2015/12/mckaysavage497863693credit_mckaysavageprayer_flag_pole_with_lhotse_and_everestnepal.jpg',
        },
        {
          src: 'https://c0.wallpaperflare.com/preview/253/954/418/camping-camp-adventure-the-stake.jpg',
        },
        {
          src: 'https://www.jakpost.travel/wimages/large/231-2310119_mountain-trekking.jpg',
        },
        {
          src: 'https://da8qcmjpujrcg.cloudfront.net/media/marketplace/images/70/DSC_0647.JPG',
        },
      ],
    }
  },
};
</script>
