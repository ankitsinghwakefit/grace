<template>
<div class="mynuxt">
  <Navbar />
  <Hero />
  <Feature />
  <Carousal />
  <Intro />
  <Footer />
</div>
  
</template>

<script>
export default {
  head: {
    title: 'Best Workation Himachal Pradesh',
    meta: [
      {
        hid: 'description',
        name: 'description',
        content: 'Homestays in himachal pradesh'
      },
    ],
  }
}
</script>

<style>

/* .container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
 */
@import url('https://fonts.googleapis.com/css2?family=Lobster&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Andika+New+Basic:ital,wght@0,400;0,700;1,400;1,700&display=swap');
.mynuxt {
  font-family: 'Andika New Basic', sans-serif !important;
}
.vue-typer .custom.char {
  font-size: 30px;
  color: #373445 ;
  font-weight: bolder;
  background-color: #AB9856;
}
.vue-typer .custom.char.selected {
  background-color: #AB9856;
}

.vue-typer .custom.caret {
  width: 10px;
  background-color: palevioletred;
}
@media only screen and (max-width: 900px) {
  .vue-typer .custom.char {
  font-size: 25px;
  color: #373445 ;
  font-weight: bolder;
  background-color: #AB9856;
}
.vue-typer .custom.char.selected {
  background-color: #AB9856;
}

.vue-typer .custom.caret {
  width: 10px;
  background-color: palevioletred;
}
}
@media only screen and (max-width: 768px) {
  .vue-typer .custom.char {
  font-size: 20px;
  color: #373445 ;
  font-weight: bolder;
  background-color: #AB9856;
}
.vue-typer .custom.char.selected {
  background-color: #AB9856;
}

.vue-typer .custom.caret {
  width: 10px;
  background-color: palevioletred;
}
}
</style>
