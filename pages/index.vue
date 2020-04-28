<template>
  <v-carousel cycle height="600" hide-delimiter-background show-arrows-on-hover>
    <v-carousel-item v-for="(slide, i) in slides" :key="i">
      <v-img :src="slide"></v-img>
    </v-carousel-item>
  </v-carousel>
</template>

<script>
export default {
  components: {},
  data() {
    return {
      slides: ['deglo.jpg', 'frosch.png', 'viervier.png']
    }
  }
}
</script>
