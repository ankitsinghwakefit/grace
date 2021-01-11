<template>
  <div class="colorService">
      <h1 class="title-with-line text-center mb-5 myHead">Attractions Nearby Homestay</h1>
    <div class="container">
      <!-- <div class="row mb-2 justify-content-center text-center">
        <div class="col-lg-4">
          <span class="caption">Our Services</span>
        </div>
      </div> -->
      <div class="row mt-2">
        <div class="col-lg-4 col-md-6">
          <div class="feature-1">
            <div class="iconContainer">
                <div class="icon-wrapper bg-primary text-center setIcon">
             <i class="fas fa-campground"></i>
            </div>
            </div>
            <div class="feature-1-content">
                <h2><span class="attraction-Name">Triund</span></h2>
                <p class="para">A trekker’s delight, Triund is a scenic hill station located at a height of 2,828 meters above sea level. From this place, you can get picture-perfect views of the Kangra Valley on one side and the Dhauladhar Range on the other.</p>
                <p>
                    <a href="#" class="btn px-4 ">Learn More</a>
                </p>
            </div>
          </div>
        </div>
        <div class="col-lg-4 col-md-6">
          <div class="feature-1">
            <div class="iconContainer">
                <div class="icon-wrapper bg-primary text-center setIcon">
             <i class="fas fa-swimmer"></i>
            </div>
            </div>
            <div class="feature-1-content">
                <h2><span class="attraction-Name">Bhagsu Waterfall</span></h2>
                <p class="para">With its sparkling waters and rocky background, the stunning Bhagsu Waterfall is among the most mesmerizing destinations to explore in and around Kangra.</p>
                <p>
                    <a href="#" class="btn px-4 ">Learn More</a>
                </p>
            </div>
          </div>
        </div>
        <div class="col-lg-4 col-md-6">
          <div class="feature-1">
            <div class="iconContainer">
                <div class="icon-wrapper bg-primary text-center setIcon">
             <i class="fas fa-gopuram"></i>
            </div>
            </div>
            <div class="feature-1-content">
                <h2><span class="attraction-Name">Mcleodganj</span></h2>
                <p class="para">Located a short drive away from Kangra, Mcleodganj is famous as the abode of the Tibetan Spiritual leader Dalai Lama. Fringed by lush greenery and lofty hills, the culturally rich town showcases a deep Tibetan influence.</p>
                <p>
                    <a href="#" class="btn px-4 ">Learn More</a>
                </p>
            </div>
          </div>
        </div>
      <!-- </div>
      <div class="row mt-2"> -->
        <div class="col-lg-4 col-md-6">
          <div class="feature-1">
            <div class="iconContainer">
                <div class="icon-wrapper bg-primary text-center setIcon">
             <i class="fas fa-baseball-ball"></i>
            </div>
            </div>
            <div class="feature-1-content">
                <h2><span class="attraction-Name">Dharamshala Cricket Stadium</span></h2>
                <p class="para">Nestled in the lap of the majestic Himalayan mountain range lies the quaint Dharamshala Cricket Stadium, it is one of the highest sports grounds in the world.</p>
                <p>
                    <a href="#" class="btn px-4 ">Learn More</a>
                </p>
            </div>
          </div>
        </div>
        <div class="col-lg-4 col-md-6">
          <div class="feature-1">
            <div class="iconContainer">
                <div class="icon-wrapper bg-primary text-center setIcon">
             <i class="fas fa-fire"></i>
            </div>
            </div>
            <div class="feature-1-content">
                <h2><span class="attraction-Name">Jwala Devi Temple</span></h2>
                <p class="para">The serene valley of Kangra is where the eternal flames of the Jwala Devi Temple burn incessantly and attract countless pilgrims from all over India to witness this mystical occurrence.</p>
                <p>
                    <a href="#" class="btn px-4 ">Learn More</a>
                </p>
            </div>
          </div>
        </div>
        <div class="col-lg-4 col-md-6">
          <div class="feature-1">
            <div class="iconContainer">
                <div class="icon-wrapper bg-primary text-center setIcon">
             <i class="fas fa-seedling"></i>
            </div>
            </div>
            <div class="feature-1-content">
                <h2><span class="attraction-Name">Tea Bagan</span></h2>
                <p class="para">Palampur is a green hill station and a municipal council in the Kangra Valley in the Indian state of Himachal Pradesh, surrounded by tea gardens and pine forests before they merge with the Dhauladhar ranges. </p>
                <p>
                    <a href="#" class="btn px-4 ">Learn More</a>
                </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.myHead {
   color: #373445;
  width: 100%;
  font-size: 40px;
  margin-bottom: 40px;
  font-weight: bolder;
}
.para {
    color: palevioletred;
}
.btn {
    background-color: palevioletred;
    color: papayawhip;
}
.attraction-Name {
  color: palevioletred;
  font-weight: bolder;
}
i {
    color: cornsilk;
}
.colorService {
     background-color: #e7d4c0;
    padding-top: 30px;
}
.iconContainer {
    margin: 0 auto;
}
.bg-primary {
    background-color: #5577B4 !important;
}
.btn-primary{
       background-color: #5577B4 !important;
 
}
.setIcon {
    height: 90px;
    width: 40%;
    margin: 0 auto;
    font-size: 30px;
    display: flex;
     justify-content: center;
  align-items: center;
  text-align: center;
clip-path: polygon(50% 0%, 80% 10%, 100% 35%, 100% 70%, 80% 90%, 50% 100%, 20% 90%, 0% 70%, 0% 35%, 20% 10%);
}
.caption {
  color: #5577b4;
  text-transform: uppercase;
  font-size: 11px;
  letter-spacing: 0.2rem;
  font-weight: 700;
}
.feature-1,
.person {
  background: #fff;
  margin-bottom: 20px;
  padding-top: 20px;
}
.feature-1-content {
    padding: 50px 20px 20px 20px;
    text-align: center;
}
@media only screen and (max-width: 900px) {
  .myHead {
 
  font-size: 35px;
}
}
@media only screen and (max-width: 768px) {
 .myHead {
  font-size: 25px;
}
}
</style>
