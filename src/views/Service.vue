
    <template>
<v-app id="recent">
     <v-row class="text-center">
    <v-col class="mb-4">
      <h1 class="display-2 font-weight-bold mb-3 red--text">{{$route.params.services}}</h1>

      <p class="subheading font-weight-regular">
        {{content}}
      </p>
  
    </v-col>
  </v-row>
</v-app>
</template>
<script>
export default {
  data: function() {
    return{
      content: ''
    }
  },
  mounted(){
    this.getApiData()
  },
  methods: {
    getApiData(){
     fetch('https://fakerapi.it/api/v1/texts?_quantity=1&_characters=500')
        .then(response => response.json())
        .then(data => {
          this.content = data.data[0].content;
        }).catch(err => console.log(err))
    }
  }
}
</script>