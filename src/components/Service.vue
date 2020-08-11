 <template>
 <v-app id="service">
     <v-container>
  <v-row class="text-center">
    <v-col class="mb-4">
      <h1 class="display-2 font-weight-bold mb-3 red--text">What we do?</h1>

      <p class="subheading font-weight-regular">
        Quickly build an effective pricing table for your potential customers
        <br/>with this layout. It's built with default Material-UI components with
        <br/>little customization.
      </p>
    </v-col>
  </v-row>
  <v-card class="d-inline-flex text-center"  width="500" height="300" 
         v-for="item in servicesArr" :key="item.name"  :to="item.path"
           type="button"  v-bind:style='{ backgroundImage: "url(" + item.url + ")", }'>
          <span class="recent-item">{{item.name}}</span>
        
      
  </v-card>
     </v-container>
 </v-app>
</template>
      <script>
export default {
  name: "Services",
  data: function () {
    return {
      servicesArr: [
        {
          name: "Skiing",
          url:
            "https://img3.oastatic.com/img2/40917734/600x300r/rehjan-latu-ura-9-km-kajaani-finland.jpg",
          path: "skiing",
        },

        {
          name: "Trekking (backpacking)",
          url:
            "https://di-uploads-pod5.dealerinspire.com/triplejsaipan/uploads/2019/03/Three-People-Hiking-Up-Mountain_24359265.jpg",
          path: "trekking",
        },
        {
          name: "Mountain Biking",
          url:
            "https://bikefeatures.com/wp-content/uploads/2018/07/Best-Mountain-Bikes-Under-1000.jpg",
          path: "moutainbiking",
        },
        {
          name: "Local Sight Seeing",
          url:
            "https://assets.traveltriangle.com/blog/wp-content/uploads/2016/02/manali-river-beas.jpg",
          path: "localsightseeing",
        },
        {
          name: "Jeep Safari",
          url:
            "https://www.picnicwale.com/assets/adventure/manali-jeep-safari-season.jpg",
          path: "jeepsafari",
        },
        {
          name: "Expedition Climbing",
          url:
            "https://www.alpineinstitute.com/media/274036/denali_expedition_climbing_summit_ridge.jpg",
          path: "expeditionclimbing",
        },
        {
          name: "Family Trips",
          url:
            "https://i.pinimg.com/736x/24/61/03/246103a96862eeab2dc50a74a7de8cac.jpg",
          path: "familytrips",
        },
        {
          name: "Day Hikes",
          url:
            "https://img.traveltriangle.com/blog/wp-content/uploads/2019/04/Trekking-In-Himachal-Pradesh-cover.jpg",
          path: "dayhikes",
        },
        {
          name: "Canyoning",
          url:
            "https://bluberryholidays.com/wp-content/uploads/2020/05/a8apdxyy5wmrddt.jpg",
          path: "canyoning",
        },
        {
          name: "Cycling",
          url:
            "https://www.bbcgoodfood.com/sites/default/files/editor_files/2020/05/cycling_3.jpg",
          path: "cycling",
        },
      ],
    };
  },
};
</script>
