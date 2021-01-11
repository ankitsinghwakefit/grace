<template>
  <div class="featurecontainer">
    <b-container class="">
      <b-row>
        <h1 class="featureheading">
           Our Homestays in himachal pradesh
        </h1>
      </b-row>

      <b-row>
        <b-col xl="6" lg="6" md="12" sm="12" class="mt-4">
          <b-card no-body class="overflow-hidden" style="max-width: 540px;">
            <b-row no-gutters>
              <b-col md="6">
                <b-card-img
                  src="~assets/bed.jpg"
                  alt="Image"
                  class="rounded-0"
                ></b-card-img>
              </b-col>
              <b-col md="6">
                <b-card-body title="Accommodation.">
                  <b-card-text>
                      <b-badge variant="primary"
                      ><i class="fas fa-home"></i
                    ></b-badge>
                    Comfortable Stay.<br />
                    <b-badge variant="danger"
                        ><i class="fab fa-periscope"></i></b-badge>
                    Kangra valley Himachal
                    Pradesh.<br />
                    <b-badge variant="success"
                        ><i class="fas fa-first-aid"></i></b-badge>
                    Clean and Hygienic Rooms.<br />
                    <b-badge variant="warning"
                        ><i class="fas fa-taxi"></i></b-badge>
                    Pick up & Drop off
                  </b-card-text>
                </b-card-body>
              </b-col>
            </b-row>
          </b-card>
        </b-col>
        <b-col xl="6" lg="6" md="12" sm="12" class="mt-4">
          <b-card no-body class="overflow-hidden" style="max-width: 540px;">
            <b-row no-gutters>
              <b-col md="6">
                <b-card-img
                  src="~assets/outdor.jpg"
                  alt="Image"
                  class="rounded-0"
                ></b-card-img>
              </b-col>
              <b-col md="6">
                <b-card-body title="Outdoor Adventure.">
                  <b-card-text>
                    <span class="fun"
                      ><b-badge variant="danger"
                        ><i class="fab fa-free-code-camp"></i></b-badge>
                      Bonfire</span
                    >
                    <br />
                    <span class="fun"
                      ><b-badge variant=""
                        ><i class="fas fa-mountain"></i
                      ></b-badge>
                      Trekking</span
                    >
                    <br />
                    <span class="fun"
                      ><b-badge variant="success"
                        ><i class="fas fa-campground"></i
                      ></b-badge>
                      Camping</span
                    ><br />
                    <span class="fun"
                      ><b-badge variant="primary"
                        ><i class="fas fa-star-half-alt"></i></b-badge>
                      Stargazing</span
                    >
                    <br />
                    <span class="fun"
                      ><b-badge variant="info"
                        ><i class="fas fa-walking"></i></b-badge>
                      Village Walking Trails</span
                    >
                    <br />
                  </b-card-text>
                </b-card-body>
              </b-col>
            </b-row>
          </b-card>
        </b-col>
      </b-row>
     
      <b-row>
        <b-col xl="6" lg="6" md="12" sm="12" class="mt-4">
          <b-card no-body class="overflow-hidden" style="max-width: 540px;">
            <b-row no-gutters>
              <b-col md="6">
                <b-card-img
                  src="~assets/meals.jpg"
                  alt="Image"
                  class="rounded-0"
                ></b-card-img>
              </b-col>
              <b-col md="6">
                <b-card-body title="Healthy and Fresh Meals.">
                  <b-card-text>
                      <span class="fun"
                      >
                      <b-badge variant="danger"
                      ><i class="fas fa-mug-hot"></i
                    ></b-badge>
                    Tea, Breakfast, Lunch & Dinner.</span><br />
                    <span class="fun"
                      ><b-badge variant="success"
                        ><i class="fas fa-thumbs-up"></i></b-badge>
                      Tasty & Healthy</span
                    >
                    <br />
                    <span class="fun"
                      ><b-badge variant="danger"
                        ><i class="far fa-heart"></i></b-badge>
                      Local flavors</span
                    >
                    <br />
                  </b-card-text>
                </b-card-body>
              </b-col>
            </b-row>
          </b-card>
          
        </b-col>
        <b-col xl="6" lg="6" md="12" sm="12" class="mt-4">
          <b-card no-body class="overflow-hidden" style="max-width: 540px;">
            <b-row no-gutters>
              <b-col md="6">
                <b-card-img
                  src="~assets/wifi3.jpg"
                  alt="Image"
                  class="rounded-0"
                ></b-card-img>
              </b-col>
              <b-col md="6">
                <b-card-body title="Hi-Speed Wifi.">
                  <b-card-text>
                    <b-badge variant="info"
                      ><i class="fas fa-wifi"></i
                    ></b-badge>
                    Hi-Speed Internet.<br />
                    <b-badge variant="success"
                      ><i class="fas fa-medkit"></i></b-badge>
                    First-Aid.<br />
                    <b-badge variant="secondary"
                      ><i class="fas fa-laptop-house"></i
                    ></b-badge>
                    WFH Setup.
                  </b-card-text>
                </b-card-body>
              </b-col>
            </b-row>
          </b-card>
        
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Andika+New+Basic:ital,wght@0,400;0,700;1,400;1,700&display=swap");
.card-text {
  color: #373445;
  font-size: 20px;
}
.home {
  text-decoration: line-through;
  color: brown;
  font-weight: bolder;
}
.fun {
  color: brown;
  font-weight: bolder;
}
.card-header {
  background-color: #658ea9;
  color: #373445;
  font-size: 25px;
  font-weight: bolder;
}
.featurecontainer {
  background-color: #e7d4c0;
  padding-bottom: 50px;
  font-family: "Andika New Basic", sans-serif;
}
.featureheading {
  color: #373445;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  width: 100%;
  font-size: 40px;
  margin-top: 35px;
  margin-bottom: 40px;
  font-weight: bolder;
}
@media only screen and (max-width: 900px) {
  .featureheading {
  font-size: 35px;
}
}
@media only screen and (max-width: 768px) {
  .featureheading {
  font-size: 25px;
}
}
</style>
