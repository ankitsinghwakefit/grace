<template>
    <div>
        <Navbar />
        <!-- <div class="jumbo-Container">
      <b-jumbotron>
        <template #header>Contact</template>
        <template #lead>
          Our team is working really hard to give you lifetime memories.
          <br>
          We are just a miscall away, Give it on <span class="contactus">98997 12768</span>.
          <br>
          Also, write to us at <span class="contactus">muktilisten@gmail.com</span>
          
        </template>
        <ContactForm />
        <hr class="my-4" />

        <p>
          We entertain your requests within 2 Minutes, Let's try!
        </p>
        <b-link class="button" to="/about" style="vertical-align:middle"><span>About us</span></b-link>
        <b-link class="button" to="/services" style="vertical-align:middle"><span>Services</span></b-link>
        
      </b-jumbotron>
    </div> -->
    <div class="myContainer">
      <div class="myChildContainer">
        <div class="childParent">
        <h2 class="myh2">Contact Us</h2>
        <div class="contents">
          Our team is working really hard to give you lifetime memories.
          <br>
          <i class="fas fa-phone-square-alt"></i> <span class="contactus">+91 98997 12768</span> |
          <i class="fas fa-envelope"></i> <span class="contactus">muktilisten@gmail.com</span>
          
        </div>
        <ContactForm />
        <hr class="my-4" />

        <p>
          We entertain your requests within 2 Minutes, Let's try!
        </p>
        <b-link class="button" to="/about" style="vertical-align:middle"><span>About us</span></b-link>
        <b-link class="button" to="/services" style="vertical-align:middle"><span>Services</span></b-link>
        </div>
      </div>
    </div>
    <Footer />
    </div>
</template>

<style scoped>
i {
  font-size: 18px;
}
.contactus {
  font-weight: bolder;
  color: palevioletred;
  font-size: 18px;
}
.contents {
  font-size: 18px;
  padding: 18px 0;
  line-height: 1.5;
}
.jumbotron {
    background-color:#373445 !important; 
    color : #AB9856;
}
.myContainer {
  background-color:#373445 !important; 
    color : #AB9856;
  margin-bottom: 30px;
}
.childParent {
  padding: 20px;
}
.myh2 {
  font-size: 60px;
  margin: 20px 0;
}

.button {
  display: inline-block;
  border-radius: 8px;
  background-color: #AB9856;
  border: none;
  color: #373445;
  text-align: center;
  font-size: 20px;
  padding: 10px;
  width: 230px;
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

@media only screen and (max-width: 380px) { 
.contactFrom {
  width: 350px;
}
}
@media only screen and (max-width: 600px) { 
.contactFrom {
  width: 450px;
}
.contents {
  font-size: 14px;
  padding: 18px 0;
  line-height: 1.5;
}
.button {
  display: inline-block;
  border-radius: 8px;
  background-color: #AB9856;
  border: none;
  color: #373445;
  text-align: center;
  font-size: 16px;
  padding: 10px;
  width: 160px;
  transition: all 0.5s;
  font-weight: bolder;
  cursor: pointer;
  margin: 5px;
}
p {
  font-size: 14px;
}
}
.jumbo-Container {
   width: 60%;
   margin: 0 auto;
}
.myChildContainer {
  width: 100%;
  margin: 0 auto;
  display: flex;
  align-items: center;
  justify-content: center;
}
@media only screen and (max-width: 900px) { 
.contents {
  font-size: 16px;
  padding: 18px 0;
  line-height: 1.5;
}
.button {
  display: inline-block;
  border-radius: 8px;
  background-color: #AB9856;
  border: none;
  color: #373445;
  text-align: center;
  font-size: 18px;
  padding: 10px;
  width: 200px;
  transition: all 0.5s;
  font-weight: bolder;
  cursor: pointer;
  margin: 5px;
}
p {
  font-size: 15px;
}

}
</style>