<template>
  <div>
    <bar />
    <carousel />
    <lorem />
    <barslike />
    <br>
    <brendovi />
  </div>
</template>

<script>
import Carousel from '@/components/Carousel.vue'
import Bar from '@/components/Bar.vue'
import Lorem from '@/components/Lorem.vue'
import Barslike from '@/components/Barslike.vue'
import Brendovi from '@/components/Brendovi.vue'

export default {
  components: {
    Carousel,
    Bar,
    Lorem,
    Barslike,
    Brendovi,
  }
}
</script>
