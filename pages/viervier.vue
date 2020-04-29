<template>
  <div>
    <mainContent :title="title" :picture="picture" :sections="sections" />

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
      title: 'Steinenvorstadt',
      picture: { src: 'viervier.png', alt: 'Steine Hänger' },
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
          title: 'Regula',
          text: 'D Regula stellt klar das si d Froge selber stellt.',
          link: 'https://youtu.be/3YZKiUrW5-4?t=1114'
        },
        {
          title: '44er',
          text: 'Wiso musme fast e Pistole im Sagg drage?',
          link: 'https://youtu.be/3YZKiUrW5-4?t=1114'
        },
        {
          title: 'Jugendhus',
          text: 'Wie stoht ums Jugendhus in Basel?',
          link: 'https://youtu.be/3YZKiUrW5-4?t=1114'
        }
      ]
    }
  }
}
</script>

<style scoped></style>
