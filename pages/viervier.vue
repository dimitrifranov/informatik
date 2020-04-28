<template>
  <div>
    <h1 class="mb-3">{{ title }}</h1>

    <v-img
      :src="picture"
      class="parallax float-md-left"
      height="500"
      :alt="alt"
    ></v-img>
    <v-expansion-panels class="parallax float-md-right mt-3" hover popout>
      <v-expansion-panel v-for="(item, i) in items" :key="i">
        <v-expansion-panel-header>{{ item.title }}</v-expansion-panel-header>
        <v-expansion-panel-content>{{
          item.content
        }}</v-expansion-panel-content>
      </v-expansion-panel>
    </v-expansion-panels>

    <v-rating class="float-md-right"></v-rating>

    <h2 class="divider py-3">Highlights</h2>
    <v-timeline>
      <v-timeline-item>
        <v-card>
          <v-card-title>Regula</v-card-title>
          <v-card-text
            >D Regula stellt klar das si d Froge selber stellt.</v-card-text
          >
          <v-card-actions
            ><v-btn href="https://youtu.be/3YZKiUrW5-4?t=1114"
              >Video<v-icon right>mdi-play-circle-outline</v-icon></v-btn
            ></v-card-actions
          >
        </v-card>
      </v-timeline-item>
      <v-timeline-item>
        <v-card>
          <v-card-title>44er</v-card-title>
          <v-card-text>Wiso musme fast e Pistole im Sagg drage?</v-card-text>
          <v-card-actions
            ><v-btn href="https://youtu.be/3YZKiUrW5-4?t=1114"
              >Video<v-icon right>mdi-play-circle-outline</v-icon></v-btn
            ></v-card-actions
          >
        </v-card>
      </v-timeline-item>
      <v-timeline-item>
        <v-card>
          <v-card-title>Jugendhus</v-card-title>
          <v-card-text>Wie stoht ums Jugendhus in Basel?</v-card-text>
          <v-card-actions
            ><v-btn href="https://youtu.be/3YZKiUrW5-4?t=1114"
              >Video<v-icon right>mdi-play-circle-outline</v-icon></v-btn
            ></v-card-actions
          >
        </v-card>
      </v-timeline-item>
    </v-timeline>
  </div>
</template>

<script>
export default {
  data() {
    return {
      title: 'Steinenvorstadt',
      picture: 'viervier.png',
      alt: 'Deglo Onete',
      items: [
        {
          title: 'Hintergründ',
          content:
            'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'
        },
        {
          title: 'Gschicht',
          content:
            'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'
        },
        {
          title: 'Ahwändige',
          content:
            'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'
        },
        {
          title: 'Ähnliches',
          content:
            'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'
        }
      ]
    }
  }
}
</script>

<style scoped></style>
