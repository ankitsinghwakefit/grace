<template>
    <div>
        <Navbar />
        <div class="jumbo-Container">
      <b-jumbotron>
        <template #header>Services</template>

        <template #lead>
          Happy Journey, We are here looking forward to welcoming you!<br>
          <ul>
              <li>Double bedroom with 1-2 windows for memories.</li>
              <li>Chair, table & 24*7 high-speed wireless wifi.</li>
              <li>Complete work from home setup with room heaters.</li>
              <li>24*7 Electricity, water heaters & blankets.</li>
              <li>Tea, breakfast, lunch & dinner.</li>
              <li>Pickup & drop facilities to airport or bus stand.</li>
          </ul>
          
        </template>
        
        <hr class="my-4" />

        <p>
          On-demand Paragliding, Trekking & camping services to gather more memories.
        </p>
        <b-link class="button" to="/contact" style="vertical-align:middle"><span>Book Mukti!</span></b-link>
        <b-link class="button" to="/" style="vertical-align:middle"><span>Home</span></b-link>
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
/* .jumbo-Container {
    margin-top: 40px;
} */
</style>