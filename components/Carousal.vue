<template>
<div class="mt-4 mb-4 container">
   <b-row class="mb-4">
    <b-col><b-img src="~/assets/heronew.jpg" fluid-grow alt="Responsive image"></b-img></b-col>
    <b-col><b-img src="~/assets/1new.jpg" fluid-grow alt="Responsive image"></b-img></b-col>
    <b-col><b-img src="~/assets/2n.jpg" fluid-grow alt="Responsive image"></b-img></b-col>
  </b-row>
  <b-row>
    <b-col><b-img src="~/assets/3n.jpg" fluid-grow alt="Responsive image"></b-img></b-col>
    <b-col><b-img src="~/assets/4n.jpg" fluid-grow alt="Responsive image"></b-img></b-col>
  </b-row>
</div>
  <!-- <div class="container myclass">
    <b-carousel
      id="carousel-1"
      v-model="slide"
      :interval="4000"
      controls
      indicators
      background="#ababab"
      img-width="1024"
      img-height="480"
      style="text-shadow: 1px 1px 2px #333;"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >

      <b-carousel-slide img-src="~/assets/1.jpg"></b-carousel-slide>
      <b-carousel-slide img-src="~/assets/2.jpg"></b-carousel-slide>
      <b-carousel-slide img-src="~/assets/3.jpg"></b-carousel-slide>
      <b-carousel-slide img-src="~/assets/4.jpg"></b-carousel-slide>
      <b-carousel-slide img-src="~/assets/5.jpg"></b-carousel-slide>

      
    </b-carousel>
    <a target="_blank" href="https://www.solobackpacker.com/offbeat-kangra-valley/">Image Source</a>
  </div> -->
</template>

<script>
  export default {
    data() {
      return {
        slide: 0,
        sliding: null
      }
    },
    methods: {
      onSlideStart(slide) {
        this.sliding = true
      },
      onSlideEnd(slide) {
        this.sliding = false
      }
    }
  }
</script>

<style scoped>
.myclass {
    margin-top: 20px;
    margin-bottom: 20px;
     
}
</style>