<template>
  <div>
    <mainContent :title="title" :picture="picture" :sections="sections" />

    <v-btn
      left
      rounded
      large
      color="purple"
      class="ma-3"
      href="https://www.instagram.com/degloonete/"
    >
      Instagram Account
    </v-btn>
  </div>
</template>

<script>
import mainContent from '@/components/mainContent.vue'
export default {
  components: {
    mainContent
  },
  data() {
    return {
      title: 'Deglo Onete',
      picture: { src: 'deglo.jpg', alt: 'Deglo Onete' },
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
      ]
    }
  }
}
</script>

<style scoped></style>
