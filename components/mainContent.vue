<template>
  <div>
    <h1 class="mb-3">
      {{ title }}
    </h1>

    <v-img
      :src="picture.src"
      class="parallax float-md-left mb-5"
      height="500"
      :alt="picture.alt"
    />
    <v-expansion-panels class="parallax float-md-right mt-3" hover popout>
      <v-expansion-panel v-for="(section, i) in sections" :key="i">
        <v-expansion-panel-header>{{ section.title }}</v-expansion-panel-header>
        <v-expansion-panel-content>
          {{ section.content }}
        </v-expansion-panel-content>
      </v-expansion-panel>
    </v-expansion-panels>

    <v-rating class="float-md-right" />
    <v-divider class="divider mb-5" />
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      required: true
    },
    sections: {
      type: Array,
      default() {
        return [
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
    },
    picture: {
      type: Object,
      default() {
        return {
          src: 'deglo.jpg',
          alt: 'Deglo Onete'
        }
      }
    }
  }
}
</script>

<style scoped>
@media only screen and (min-width: 900px) {
  .parallax {
    width: 49%;
  }

  .divider {
    clear: both;
  }
}
</style>
