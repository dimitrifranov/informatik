<template>
  <div>
    <h2 class="mb-3">
      Alli wichtige Insider erklärt
    </h2>
    <v-carousel
      cycle
      height="50vh"
      hide-delimiter-background
      show-arrows-on-hover
    >
      <v-carousel-item v-for="(slide, i) in slides" :key="i">
        <v-img :src="slide" />
      </v-carousel-item>
    </v-carousel>
    <v-img class="parallax mt-6 float-md-left" src="hang_out.svg" />
    <div class="float-md-right parallax">
      <p class="ma-6">
        Kensches wenn du mit neue lüt chillsch und dich nit würklich integriert
        fühlsch will du d Insider nid kennsch?
      </p>
      <p class="ma-6">
        Mir wenn das das in unserem Fründeskreis nümm passiert!
      </p>
      <p class="ma-6">
        Wägä dem gits die Sitte, um dir die wichtigste Insider zerkläre.
      </p>
    </div>
    <v-img class="parallax mt-6 float-md-right divider" src="having_fun.svg" />
    <div class="float-md-left parallax">
      <p class="ma-6">
        Mit dem wo du do lernsch chasch du dini Ziit mit uns gniesse und über
        die gliche Witz lache wie mir!
      </p>
      <p class="ma-6">
        Start jetzt mit eim vo dä wichtigste Insiders...
      </p>
      <v-btn color="purple" to="deglo">
        Erfahr meh überd Deglo Onete
      </v-btn>
    </div>
  </div>
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
