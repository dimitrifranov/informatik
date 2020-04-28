<template>
  <div>
    <h1 class="mb-3">{{ title }}</h1>

    <v-img
      :src="picture"
      class="parallax float-md-left"
      height="500"
      :alt="alt"
    ></v-img>
    <v-expansion-panels
      class="parallax float-md-right mt-3"
      hover="true"
      popout="true"
    >
      <v-expansion-panel v-for="(item, i) in items" :key="i">
        <v-expansion-panel-header>{{ item.title }}</v-expansion-panel-header>
        <v-expansion-panel-content>{{
          item.content
        }}</v-expansion-panel-content>
      </v-expansion-panel>
    </v-expansion-panels>

    <v-rating class="float-md-right"></v-rating>
  </div>
</template>

<script>
export default {
  data() {
    return {
      title: 'Basler Ultras',
      picture: 'frosch.png',
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

<style lang="scss" scoped></style>
