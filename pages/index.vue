<template>
  <v-carousel cycle height="400" hide-delimiter-background show-arrows-on-hover>
    <v-carousel-item v-for="(slide, i) in slides" :key="i"></v-carousel-item>
  </v-carousel>
</template>

<script>
export default {
  components: {}
}
</script>
