<template>
    <div>
        <Navbar />
        <div class="jumbo-Container">
      <b-jumbotron>
        <template #header>Contact</template>

        <template #lead>
          Our team is working really hard to give you lifetime memories.
          <br>
          We are just a miscall away, Give it on <span class="contactus">72249 53427</span>.
          <br>
          Also, write to us at <span class="contactus">muktilisten@gmail.com</span>
          
        </template>
        
        <hr class="my-4" />

        <p>
          We entertain your requests within 2 Minutes, Let's try!
        </p>
        <b-link class="button" to="/about" style="vertical-align:middle"><span>About us</span></b-link>
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
.contactus {
  font-weight: bolder;
  color: palevioletred;
}
/* .jumbo-Container {
    margin-top: 40px;
} */
</style>