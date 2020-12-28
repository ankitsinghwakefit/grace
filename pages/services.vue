<template>
  <div>
    <particles-bg type="circle" :bg="true" />
    <Navbar />
    <div class="mycontainer">
      <b-row>
        <b-col sm="12" lg="6" xl="6" md="12">
          <b-jumbotron>
            
            <template #header>Services</template>

            <template #lead>
              Happy Journey, We are here looking forward to welcoming you!<br />
              <ul>
                <li>Meals<i class="fas fa-concierge-bell"></i> + Accommodation<i class="fas fa-home"></i>.</li>
                <li>
                  The room comes with cosy comfortable beddings, and stunning
                  mountain views.
                </li>
                <li>Double bedroom with 1-2 windows for memories.</li>

                <li>24*7 Hi-Speed WiFi, laptop-friendly workspace.</li>
                <li>Complete work from home setup with room heaters.</li>
                <li>Free parking on premises, water heaters & blankets.</li>
                <li>Tea, breakfast, lunch & dinner.</li>
                <li>Pickup & drop facilities to airport or bus stand.</li>
              </ul>
            </template>

            <hr class="my-4" />

            <p>
              On-demand Paragliding, Trekking & camping services to gather more
              memories.
            </p>
            <b-link class="button" to="/contact" style="vertical-align:middle"
              ><span>Book Mukti!</span></b-link
            >
            <b-link class="button" to="/" style="vertical-align:middle"
              ><span>Home</span></b-link
            >
            <!-- <b-button variant="primary" href="#">Do Something</b-button>
        <b-button variant="success" href="#">Do Something Else</b-button> -->
          </b-jumbotron>
        </b-col>
        <b-col sm="12" lg="6" xl="6" md="12">
          <div class="ourJumbo">
        <h2 class="ourJumboH">Attractions Nearby<i class="fas fa-braille"></i></h2>

        <div>
          <i class="fab fa-periscope"></i>Kangra - Famous for diverse attractions!<br />
          <ul>
            <li>Trekker’s delight, <span class="attraction-Name">Triund</span><i class="fas fa-campground"></i></li>
            <li>
              <span class="attraction-Name">Bhagsu Waterfall</span><i class="fas fa-swimmer"></i>
            </li>
            <li><span class="attraction-Name">Andretta</span> - Picturesque haven<i class="fas fa-tree"></i></li>

            <li><span class="attraction-Name">Mcleodganj</span> - The culturally rich town<i class="fas fa-gopuram"></i></li>
            <li><span class="attraction-Name">Kaleshwar Mahadev Temple</span><i class="fas fa-om"></i></li>
            <li><span class="attraction-Name">Kareri Lake</span><i class="fas fa-water"></i></li>
            <li><span class="attraction-Name">Jwala Devi Temple</span><i class="fas fa-fire"></i></li>
            <li><span class="attraction-Name">Dharamshala Cricket Stadium</span><i class="fas fa-baseball-ball"></i></li>
            <li><span class="attraction-Name">Famous Tea Bagan</span><i class="fas fa-seedling"></i></li>
          </ul>
        </div>

        <hr class="my-4" />

        <p class="myJumboPara">
          Also Bird watching, Star gazing, Village walk, Forest walk, Yoga & Meditation.
        </p>
         <button class="buttonTravel" @click="getQuote" style="vertical-align:middle"
              ><span>Travel Support!</span></button
            >
            
        <!-- <b-link class="button" to="/contact" style="vertical-align:middle"
          ><span>Book Mukti!</span></b-link
        >
        <b-link class="button" to="/" style="vertical-align:middle"
          ><span>Home</span></b-link
        > -->
        <!-- <b-button variant="primary" href="#">Do Something</b-button>
        <b-button variant="success" href="#">Do Something Else</b-button> -->
      </div>
        </b-col>
      </b-row>
    </div>

<!-- -------------------------- modal --------------------------------- -->

  <div v-if="form.showModal" class="myModal">
    <particles-bg type="circle" :bg="true" />
    <div class="modalChild">
    <b-form @submit="onSubmit">
        <b-form-group id="input-group-1" label="Name:" label-for="input-1">
          <b-form-input
            id="input-1"
            v-model="form.name"
            type="text"
            placeholder="Enter Name"
            required
          ></b-form-input>
        </b-form-group>

        <b-form-group
          id="input-group-2"
          label="Your Number:"
          label-for="input-2"
        >
          <b-form-input
            id="input-2"
            v-model="form.number"
            type="number"
            placeholder="Enter Number"
            required
          ></b-form-input>
        </b-form-group>

        <b-form-group
          id="input-group-3"
          label="Your Msg:"
          label-for="textarea"
        >
        <b-form-textarea
        
          id="textarea"
          v-model="form.msg"
          placeholder="Are you planning weekly/Monthly..."
          rows="3"
          max-rows="6"
        ></b-form-textarea></b-form-group>

        <b-button class="mt-4" type="submit" variant="primary">Submit</b-button>
        <b-button class="mt-4" @click="closeModal" variant="primary">Close</b-button>
      </b-form>

    <!-- <button @click="closeModal">Close</button> -->
    </div>
  </div>

    <!-- --------------------------- all pacakages -------------- -->

    <!-- <div>
  <b-card
    title="Card Title"
    img-src="https://picsum.photos/600/300/?image=25"
    img-alt="Image"
    img-top
    tag="article"
    style="max-width: 20rem;"
    class="mb-2"
  >
    <b-card-text>
      Some quick example text to build on the card title and make up the bulk of the card's content.
    </b-card-text>

    <b-button href="#" variant="primary">Go somewhere</b-button>
  </b-card>
</div> -->
    <b-container>
      <b-row>
        <b-col sm="12" lg="4" xl="4" md="12">
          <b-card
            title="Weekly lodging"
            img-src="~/assets/Servics1.jpg"
            img-alt="Image"
            img-top
            tag="article"
            class="mb-2"
          >
            <i class="fas fa-home"></i>
            <i class="fas fa-utensils"></i>
            <i class="fas fa-taxi"></i>
            <i class="fas fa-wifi"></i>
            <i class="fas fa-mug-hot"></i>
            <i class="fas fa-blanket"></i>
            <i class="fas fa-fire"></i>
            <i class="fas fa-mountain"></i>

            <b-card-text>
              <i class="fas fa-rupee-sign"></i>9,900 Onwards
            </b-card-text>

            <b-button @click="getQuote"
              >Get Quotes</b-button
            >
            <!-- <b-button
              ><a target="_blank" href="https://forms.gle/uvsTYBYKvULdVvme7"
                >Get Quotes</a
              ></b-button
            > -->
          </b-card>
        </b-col>
        <b-col sm="12" lg="4" xl="4" md="12">
          <b-card
            title="Fortnightly lodging"
            img-src="~/assets/servics2.jpg"
            img-alt="Image"
            img-top
            tag="article"
            class="mb-2"
          >
            <i class="fas fa-home"></i>
            <i class="fas fa-utensils"></i>
            <i class="fas fa-taxi"></i>
            <i class="fas fa-wifi"></i>
            <i class="fas fa-mug-hot"></i>
            <i class="fas fa-blanket"></i>
            <i class="fas fa-fire"></i>
            <i class="fas fa-mountain"></i>

            <b-card-text>
              <i class="fas fa-rupee-sign"></i>18,000 Onwards
            </b-card-text>
             <b-button @click="getQuote"
              >Get Quotes</b-button
            >

            <!-- <b-button
              ><a target="_blank" href="https://forms.gle/uvsTYBYKvULdVvme7"
                >Get Quotes</a
              ></b-button
            > -->
          </b-card>
        </b-col>
        <b-col sm="12" lg="4" xl="4" md="12">
          <b-card
            title="Monthly lodging"
            img-src="~/assets/servics3.jpg"
            img-alt="Image"
            img-top
            tag="article"
            class="mb-2"
          >
            <i class="fas fa-home"></i>
            <i class="fas fa-utensils"></i>
            <i class="fas fa-taxi"></i>
            <i class="fas fa-wifi"></i>
            <i class="fas fa-mug-hot"></i>
            <i class="fas fa-blanket"></i>
            <i class="fas fa-fire"></i>
            <i class="fas fa-mountain"></i>

            <b-card-text>
              <i class="fas fa-rupee-sign"></i>30,000 Onwards
            </b-card-text>
             <b-button @click="getQuote"
              >Get Quotes</b-button
            >
            <!-- <b-button
              ><a target="_blank" href="https://forms.gle/uvsTYBYKvULdVvme7"
                >Get Quotes</a
              ></b-button
            > -->
          </b-card>
        </b-col>
      </b-row>
    </b-container>

    <div class="container caro">
      <b-carousel
        id="carousel-fade"
        style="text-shadow: 0px 0px 2px #000"
        fade
        indicators
        img-width="1024"
        img-height="480"
      >
        <b-carousel-slide
          caption="MUKTI - I"
          img-src="~/assets/pic2small.jpg"
        ></b-carousel-slide>
        <b-carousel-slide
          caption="MUKTI - II"
          img-src="~/assets/Mukti3small.jpg"
        ></b-carousel-slide>
        <b-carousel-slide
          caption="MUKTI - III"
          img-src="~/assets/Mukti1small.jpg"
        ></b-carousel-slide>
      </b-carousel>
    </div>

    <!-- ------1 st image-------------- -->

    <!-- <div class="container mycon">
    
    <b-card
    overlay
    img-src="~/assets/pic2small.jpg"
    img-alt="Card Image"
    text-variant="white"
    title="MUKTI - I"
    
  >
    
  </b-card>
  
  </div> -->
    <!-- 2nd image ------------------- -->

    <!-- <div class="container mycon">
    
    <b-card
    overlay
    img-src="~/assets/Mukti3small.jpg"
    img-alt="Card Image"
    text-variant="white"
    title="MUKTI - II"
    
  >
    
  </b-card>
  
  </div> -->
    <!-- 3rd image------------------------------- -->
    <!-- <div class="container mycon">
    
    <b-card
    overlay
    img-src="~/assets/Mukti1small.jpg"
    img-alt="Card Image"
    text-variant="white"
    title="MUKTI - III"
    
  >
    
  </b-card>
  
  </div> -->
    <Footer />
  </div>
</template>

<script>
// import { ParticlesBg } from "particles-bg-vue";
const axios = require("axios");
export default {
  data() {
    return {
      form : {
        name: "",
        number: "",
        mag: "",
         showModal : false
      }
    };
  },
  // components : {
  //  ParticlesBg
  // },
  methods: {
    getQuote(){
      this.form.showModal = true;
      console.log("im listening",this.form.showModal);
    },
    closeModal(){
      this.form.showModal = false;
    },
    onSubmit(event) {
      event.preventDefault();
      axios
        .post("https://muktiv2.herokuapp.com/", {
          name: this.form.name,
          number: this.form.number,
          msg: this.form.msg
        })
        .then(function(response) {
          
          if(response.data == "done"){
           alert("Thanks we will revert soon!")
          }
          
        })
        .catch(function(error) {
          alert("Error - Form not submitted!")
        });
        this.form.name = "";
        this.form.number = "";
        this.form.msg = "";
        // this.form.modalShow = true;
        this.form.showModal = false;
    }
  }
};
</script>

<style scoped>
.myModal{
  z-index: 990;
  position: fixed;
   top: 0%;
  left: 0%;
  width: 100vw;
  height: 100vh;
  background-color: #434246;
  opacity: .9;
}
.modalChild {
  z-index: 980;
  transform: translate(-50%, -50%);
  position: fixed;
  top: 50%;
  left: 50%;
  width: 40%;
   padding: 17px;
   border-radius: 8px;
   opacity: 1.2;
   /* font-size: 20px; */
   font-weight: bolder;
  background-color: #ffffff;
}
.attraction-Name {
  color: palevioletred;
  font-size: 24px;
  font-weight: bolder;
}
.mycontainer {
  width: 90%;
  margin: 0 auto;
  margin-top: 20px;
}
.jumbotron{
  background-color: #373445 !important;
  color: #ab9856;
}
.ourJumbo {
   background-color: #373445 !important;
  color: #ab9856;
  border-radius: 4px;
  padding: 20px;
  font-size: 18px;
  font-weight: normal;
}
.ourJumboH{
  font-size: 45px !important;
  font-weight: normal;
  margin-top: 30px;
}
.myJumboPara {
  font-size: 16px !important;
}
.button {
  display: inline-block;
  border-radius: 13px;
  background-color: #ab9856;
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
.buttonTravel {
  display: inline-block;
  border-radius: 13px;
  background-color: #ab9856;
  border: none;
  color: #373445;
  text-align: center;
  font-size: 28px;
  padding: 20px;
  width: 300px;
  transition: all 0.5s;
  font-weight: bolder;
  cursor: pointer;
  margin: 5px;
}
.buttonTravel span {
  cursor: pointer;
  display: inline-block;
  position: relative;
  transition: 0.5s;
}
.buttonTravel span:after {
  content: "\00bb";
  position: absolute;
  opacity: 0;
  top: 0;
  right: -20px;
  transition: 0.5s;
}

.buttonTravel:hover span {
  padding-right: 25px;
}

.buttonTravel:hover span:after {
  opacity: 1;
  right: 0;
}
.buttonTravel:hover {
  box-shadow: 0 12px 16px 0 rgba(0, 0, 0, 0.24),
    0 17px 50px 0 rgba(0, 0, 0, 0.19);
}
.caro {
  margin-bottom: 25px;
  margin-top: 25px;
}
a {
  color: rgb(238, 238, 238);
  text-decoration: none;
}
.card {
  background-color: #373445;
  color: #ab9856;
  border-color: none;
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
.card-text {
  font-size: 24px;
  font-weight: bolder;
  margin-top: 13px;
}
/* .rupees {
  font-size: 20px !important;
} */
/* .myIcons {
  font-size: 24px;
} */
i {
  margin: 5px;
  font-size: 24px;
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
.buttonOne {
  display: inline-block;
  border-radius: 13px;
  background-color: #ab9856;
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

.buttonOne span {
  cursor: pointer;
  display: inline-block;
  position: relative;
  transition: 0.5s;
}
.buttonOne span:after {
  content: "\00bb";
  position: absolute;
  opacity: 0;
  top: 0;
  right: -20px;
  transition: 0.5s;
}

.buttonOne:hover span {
  padding-right: 25px;
}

.buttonOne:hover span:after {
  opacity: 1;
  right: 0;
}
.buttonOne:hover {
  box-shadow: 0 12px 16px 0 rgba(0, 0, 0, 0.24),
    0 17px 50px 0 rgba(0, 0, 0, 0.19);
}
/* .myclass {
  width: 1000px;
}
.myclass img{
  width: 100%;
} */
.mycon {
  margin-bottom: 20px;
}
@media only screen and (max-width: 768px) {
  .myModal{
  z-index: 990;
  position: fixed;
   top: 0%;
  left: 0%;
  width: 100vw;
  height: 100vh;
  background-color: #434246;
  opacity: .9;
}
.modalChild {
  z-index: 980;
  transform: translate(-50%, -50%);
  position: fixed;
  top: 50%;
  left: 50%;
  width: 90%;
  
   padding: 17px;
   border-radius: 8px;
   opacity: 1.2;
   /* font-size: 20px; */
   font-weight: bolder;
  background-color: #ffffff;
}
  .ourJumbo {
   background-color: #373445 !important;
  color: #ab9856;
  border-radius: 4px;
  padding: 20px;
  font-size: 18px;
  font-weight: normal;
}
.ourJumboH{
  font-size: 30px !important;
  font-weight: normal;
  margin-top: 30px;
}
.mycontainer {
  width: 100%;
  margin: 0 0;
  margin-bottom: 20px;
}
.attraction-Name {
  color: palevioletred;
  font-size: 20px;
  font-weight: bolder;
}
.col {
  margin: 0 !important;
}
.row {
  margin: 0 !important;
}
i {
  margin: 3px;
  font-size: 22px;
}
}
@media only screen and (max-width: 900px) {
  .mycontainer {
  width: 100%;
  margin: 0 0;
  margin-bottom: 20px;
    margin-top: 20px;
}
}
@media only screen and (max-width: 350px) {
  /* .mycon {
  display: none !important;
} */
}
/* .jumbo-Container {
    margin-top: 40px;
} */
</style>
