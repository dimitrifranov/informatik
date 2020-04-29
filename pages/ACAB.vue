<template>
  <div>
    <mainContent :title="title" :picture="picture" :sections="sections" />

    <v-btn
      left
      rounded
      large
      color="purple"
      class="ma-3"
      href="https://www.youtube.com/watch?v=LUyXhbn4hTc&feature=youtu.be"
    >
      Zum Song
    </v-btn>

    <highlights :items="items" />
  </div>
</template>

<script>
import mainContent from '@/components/mainContent.vue'
import highlights from '@/components/highlights.vue'

export default {
  components: {
    mainContent,
    highlights
  },
  data() {
    return {
      title: 'ACAB - Misandope',
      picture: { src: 'acab.jpg', alt: 'acab' },
      sections: [
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
      ],
      items: [
        {
          title: 'Sali Milan',
          text: 'Die besti Begrüessig wemme ind Innestadt will',
          link: 'https://www.youtube.com/watch?v=LUyXhbn4hTc&feature=youtu.be'
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped></style>
