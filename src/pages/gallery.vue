<template>
  <div class="container__index">

    <div class="text-bold q-mb-md text-center dateToday" style="font-size: 24px">
        Gallery
    </div>

    <div class="text-center q-mb-lg"> 
      <q-btn @click="$router.push({name: 'home'})" outline label="Schedules" class="q-px-xl" />
    </div>

    <div class="row q-col-gutter-md">
        <div v-for="client in images" style="margin: 0 auto">
          <img :src="client.pathLong" style="width: 300px; height: 240px;">
        </div>
        <div v-for="client in videos" style="margin: 0 auto">
          <video width="300" height="240" controls>
            <source :src="client.pathLong" type="video/mp4"> 
          </video>
        </div>
      </div>
    </div>
</template>

<script>
import { ref } from 'vue'
export default ({
  name: 'gallery',
  components: {
  },
  data: () => ({
    images: [],
    videos: [],
  }),


  setup () {
      return {

      }
  },
  mounted() {
      this.Images(require.context('../../public/gallery/photos', true, /\.png$/));
      this.Images(require.context('../../public/gallery/photos', true, /\.jpg$/));
      this.Videos(require.context('../../public/gallery/videos', true, /\.mp4$/));

      console.log(this.Images)
  },
  methods: {
      Images(r) {
      r.keys().forEach(key => (this.images.push({ pathLong: r(key), pathShort: key })));
    },

     Videos(r) {
      r.keys().forEach(key => (this.videos.push({ pathLong: r(key), pathShort: key })));
    },
	},
})
</script>


<style scoped>


</style>

