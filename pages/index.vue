<template>
<div>
  <Navbar />
  <Hero />
  <Intro />
  <Feature />
  <Carousal />
  <Footer />
</div>
  <!-- <div class="container">
    <div>
      <Logo />
      <h1 class="title">
        MuktiV2
      </h1>
      <div class="links">
        <a
          href="https://nuxtjs.org/"
          target="_blank"
          rel="noopener noreferrer"
          class="button--green"
        >
          Documentation
        </a>
        <a
          href="https://github.com/nuxt/nuxt.js"
          target="_blank"
          rel="noopener noreferrer"
          class="button--grey"
        >
          GitHub
        </a>
      </div>
    </div>
  </div> -->
</template>

<style>
/* .container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family:
    'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
} */
@import url('https://fonts.googleapis.com/css2?family=Lobster&display=swap');

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
