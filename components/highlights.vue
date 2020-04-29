<template>
  <div>
    <h2 class="pb-3">
      Highlights
    </h2>
    <v-timeline>
      <v-timeline-item v-for="(item, i) in items" :key="i">
        <v-card>
          <v-card-title>{{ item.title }} </v-card-title>
          <v-card-text> {{ item.text }} </v-card-text>
          <v-card-actions>
            <v-btn :href="item.link">
              Video<v-icon right>
                mdi-play-circle-outline
              </v-icon>
            </v-btn>
          </v-card-actions>
        </v-card>
      </v-timeline-item>
    </v-timeline>
  </div>
</template>

<script>
export default {
  props: {
    items: {
      type: Array,
      required: true
    }
  }
}
</script>

<style lang="scss" scoped></style>
