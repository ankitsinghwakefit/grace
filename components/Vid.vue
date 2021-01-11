<template>
  <div>
    <header>
      <div class="overlay"></div>
      <video
        playsinline="playsinline"
        autoplay="autoplay"
        muted="muted"
        loop="loop"
      >
        <source
          src="https://mdbootstrap.com/img/video/Sail-Away.mp4"
          type="video/mp4"
        />
      </video>
      <div class="container h-100">
        <div class="d-flex h-100 text-center align-items-center">
          <div class="w-100 text-white">
            <p>
              Our Services :
              <vue-typer
                class="mytyper"
                :text="[
                  'Accommodation',
                  'Meals',
                  'Trekking',
                  'Paragliding',
                  'Camping'
                ]"
                :repeat="Infinity"
                :shuffle="false"
                initial-action="typing"
                :pre-type-delay="70"
                :type-delay="70"
                :pre-erase-delay="2000"
                :erase-delay="250"
                erase-style="select-all"
                :erase-on-complete="false"
                caret-animation="blink"
              ></vue-typer>
            </p>

            <h1 class="myheading">~ Work from Mountains ~</h1>
            <b-link to="/contact" class="button" style="vertical-align:middle"
              ><span>Book Mukti!</span></b-link
            >
          </div>
        </div>
      </div>
    </header>
  </div>
</template>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Lobster&display=swap");
header {
  position: relative;
  background-color: black;
  height: 75vh;
  min-height: 25rem;
  width: 100%;
  overflow: hidden;
}

header video {
  position: absolute;
  top: 50%;
  left: 50%;
  min-width: 100%;
  min-height: 100%;
  width: auto;
  height: auto;
  z-index: 0;
  -ms-transform: translateX(-50%) translateY(-50%);
  -moz-transform: translateX(-50%) translateY(-50%);
  -webkit-transform: translateX(-50%) translateY(-50%);
  transform: translateX(-50%) translateY(-50%);
}

header .container {
  position: relative;
  z-index: 2;
}

header .overlay {
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 100%;
  background-color: black;
  opacity: 0.5;
  z-index: 1;
}

/* @media (pointer: coarse) and (hover: none) {
  header {
    background: url('https://source.unsplash.com/XT5OInaElMw/1600x900') black no-repeat center center scroll;
  }
  header video {
    display: none;
  }
} */
.button {
  display: inline-block;
  border-radius: 13px;
  /* background-color: #FFA384; */
  box-shadow: 0px 4px 0px 0px palevioletred ;
  border: 1px groove palevioletred ;
  color: white;
  text-align: center;
  font-size: 28px;
  padding: 15px;
  width: 280px;
  transition: all 0.5s;
  font-weight: bolder;
  cursor: pointer;
  margin: 5px;
}

.button span {
  cursor: pointer;
  display: inline-block;
  position: relative;
  transition: 0.5s;
}

.button span:after {
  content: "\00bb";
  position: absolute;
  opacity: 0;
  top: 0;
  right: -20px;
  transition: 0.5s;
}

.button:hover span {
  padding-right: 25px;
}

.button:hover span:after {
  opacity: 1;
  right: 0;
}
button:hover {
  box-shadow: 0 12px 16px 0 rgba(0, 0, 0, 0.24),
    0 17px 50px 0 rgba(0, 0, 0, 0.19);
}
/* h1 {
    font-size: 100px;
    font-weight: bolder;
    color: #373445;
} */
.myheading {
  font-size: 60px;
  color: white;
  margin-top: 20px;
  font-family: "Lobster", cursive !important;
  font-weight: bold;
}

p {
  font-size: 30px;
  color: white;
}
@media only screen and (max-width: 900px) {
  .myheading {
    font-size: 40px;
  }
  .button {
    display: inline-block;
    border-radius: 13px;
    text-align: center;
    font-size: 28px;
    padding: 20px;
    width: 290px;
    transition: all 0.5s;
    font-weight: bolder;
    cursor: pointer;
    margin: 5px;
  }
  p {
    font-size: 25px;
  }
}
@media only screen and (max-width: 786px) {
  .myheading {
    font-size: 30px;
  }
  p {
    font-size: 20px;
  }
}
@media only screen and (max-width: 350px) {
  .button {
    display: inline-block;
    border-radius: 13px;
    text-align: center;
    font-size: 25px;
    padding: 20px;
    width: 270px;
    transition: all 0.5s;
    font-weight: bolder;
    cursor: pointer;
    margin: 4px;
  }
  h1 {
    font-size: 65px;
    font-weight: bolder;
  }
  h3 {
    font-size: 30px;
    font-family: "Lobster", cursive;
  }
  p {
    font-size: 20px;
  }
}
</style>
