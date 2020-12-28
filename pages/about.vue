<template>
  <div>
    <Navbar />
    <div class="jumbo-Container">
      <b-jumbotron>
        <template #header>About Us ;-(!)</template>

        <template #lead>
          We are a team of Mechanical Engineers & Software Developers - working remotely from Himachal Pradesh. Together we have worked on many products.<br>
          <h1>Mukti</h1>
          Mukti is not just a word but a feel for us & we want everyone to experience it.
          <ul>
              <li>We want you to feel the silence of nature & melody of birds.</li>
              <li>Escape the town, skip daily's rat race & feel yourself in nature's lap.</li>
              <li>You will be working from the village of Himachal, famous for its magical charm and spellbound beauties, lush green surroundings.</li>
          </ul>
          
        </template>
        
        <hr class="my-4" />

        <p>
          Life is very short & we must fill it with experiences. Hey, let's not forget to book your tickets.
        </p>
        <b-link class="button" to="/contact" style="vertical-align:middle"><span>Book Mukti!</span></b-link>
        <b-link class="button" to="/services" style="vertical-align:middle"><span>Services</span></b-link>
        <!-- <b-button variant="primary" href="#">Do Something</b-button>
        <b-button variant="success" href="#">Do Something Else</b-button> -->
      </b-jumbotron>
    </div>
    <Footer />
  </div>
</template>

<style scoped>
.jumbotron {
    background-color:#373445 !important; 
    color : #AB9856;
}
.button {
  display: inline-block;
  border-radius: 13px;
  background-color: #AB9856;
  border: none;
  color: #373445;
  text-align: center;
  font-size: 28px;
  padding: 20px;
  width: 250px;
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
  content: '\00bb';
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
  box-shadow: 0 12px 16px 0 rgba(0,0,0,0.24), 0 17px 50px 0 rgba(0,0,0,0.19);
}
.jumbo-Container {
    margin-top: 20px;
    margin-bottom: 20px;
}
</style>
