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
      title: 'Basler Ultras',
      picture: { src: 'frosch.png', alt: 'Deglo Onete' },
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
          title: 'Repressione',
          text: 'Wiso sind dUltras vermummt?',
          link:
            'https://www.youtube.com/watch?v=PNMnjKPPbeI&feature=youtu.be&t=4'
        },
        {
          title: 'Penalty',
          text: 'Wiso sött me em Frosch usem wäg go?',
          link:
            'https://www.youtube.com/watch?v=PNMnjKPPbeI&feature=youtu.be&t=4'
        },
        {
          title: 'Steine',
          text: 'Die beste Partys in Basel',
          link:
            'https://www.youtube.com/watch?v=PNMnjKPPbeI&feature=youtu.be&t=4'
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped></style>
