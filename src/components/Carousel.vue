<template>
  <v-carousel
    cycle
    height="400"
    hide-delimiter-background
    show-arrows-on-hover
  >
    <v-carousel-item
      v-for="slika in slike"
      :key="slika"
      :src="slika.src"
    >

    </v-carousel-item>
  </v-carousel>
</template>

<script>
  export default {
    data () {
      return {
        slike: [
          {
            src: 'CarouselSlike/1.jpg',
          },
          {
            src: 'CarouselSlike/2.jpg',
          },
          {
            src: 'CarouselSlike/3.jpg',
          },
        ],
      }
    },
  }
</script>