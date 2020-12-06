<template>
<div class="footer-container">
    <div class="footer-child">
        <div class="child-One">
            <h2>Contact</h2>
            <p>Mukti</p>
            <p>vpo khas thed</p>
            <p>Khaniyara khas,Dharamshala.</p>
        </div>
        <div class="child-One">
            <p>Tel: +91 88888 88888</p>
            <p>Email: contact@mukti.com</p>
            <p>Book a Consulation</p>
        </div>
        <div class="child-One">
            <p>Suscribe to our new offers.
            </p>
            <b-nav-form>
          <b-form-input size="sm" class="mr-sm-2" placeholder="Email"></b-form-input>
          <b-button size="sm" class="my-2 my-sm-0" type="submit">Suscribe</b-button>
        </b-nav-form>
        </div>
    </div>
</div>
  <!-- <div>
    <b-container class="myclass">
      <b-row>
        <b-col xl="4" lg="4" md="4" sm="12">1 of 3</b-col>
        <b-col xl="4" lg="4" md="4" sm="12">1 of 3</b-col>
        <b-col xl="4" lg="4" md="4" sm="12">1 of 3</b-col>
      </b-row>
    </b-container>
  </div> -->
</template>

<style scoped>
.footer-container {
    width: 100%;
    background-color: #AB9856;
    padding-top: 50px;
    padding-bottom: 50px;
}
.footer-child {
    width: 80%;
    margin: 0 auto;
    display: flex;
  justify-content: center;
  align-items: center;
  
}
.child-One {
    width: 100%;
}
@media only screen and (max-width: 700px) { 
   .footer-child {
    margin: 0 auto;
    display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
}
@media only screen and (max-width: 380px) { 
    .footer-container {
    width: 100%;
    background-color: #AB9856;
    padding-top: 50px;
    padding-bottom: 50px;
}
   .footer-child {
    margin: 0 auto;
    display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
}
</style>
