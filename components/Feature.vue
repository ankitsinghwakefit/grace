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
                  src="~assets/fea1.jpg"
                  alt="Image"
                  class="rounded-0"
                ></b-card-img>
              </b-col>
              <b-col md="6">
                <b-card-body title="Location">
                  <b-card-text>
                    <b-badge variant="danger"
                        ><i class="fab fa-periscope"></i></b-badge>
                    <span class="home">CITY</span>, a small Village - Kangra
                    (Away from cities) in Heart of Dharamshala - Himachal
                    Pradesh.
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
                  src="~assets/location.jpg"
                  alt="Image"
                  class="rounded-0"
                ></b-card-img>
              </b-col>
              <b-col md="6">
                <b-card-body title="Pick up drop off service">
                  <b-card-text>
                    <b-badge variant="success"
                        ><i class="fas fa-taxi"></i></b-badge>
                    Airport/Bus stand pick up or drop off service to avoid any
                    Inconvenience.
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
                  src="~assets/parag.jpg"
                  alt="Image"
                  class="rounded-0"
                ></b-card-img>
              </b-col>
              <b-col md="6">
                <b-card-body title="Fun on demand">
                  <b-card-text>
                    <span class="fun"
                      ><b-badge variant="success"
                        ><i class="fab fa-pied-piper-square"></i
                      ></b-badge>
                      Paragliding</span
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
                      ><b-badge variant="danger"
                        ><i class="fas fa-campground"></i
                      ></b-badge>
                      Camping</span
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
                  src="~assets/acom.jpg"
                  alt="Image"
                  class="rounded-0"
                ></b-card-img>
              </b-col>
              <b-col md="6">
                <b-card-body title="Accommodation">
                  <b-card-text>
                    <b-badge variant="success"
                      ><i class="fas fa-wifi"></i
                    ></b-badge>
                    Hi-Speed Internet.<br />
                    <b-badge variant="danger"
                      ><i class="fas fa-home"></i
                    ></b-badge>
                    Comfortable Stay.<br />
                    <b-badge variant="secondary"
                      ><i class="fas fa-laptop-house"></i
                    ></b-badge>
                    WFH Setup.<br />
                    <b-badge variant="danger"
                      ><i class="fas fa-mug-hot"></i
                    ></b-badge>
                    Tea, Breakfast, Lunch & Dinner.
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
  color: #373445;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  width: 100%;
  font-size: 35px;
  margin-top: 35px;
  margin-bottom: 40px;
  font-weight: bolder;
}
}
@media only screen and (max-width: 768px) {
  .featureheading {
  color: #373445;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  width: 100%;
  font-size: 25px;
  margin-top: 35px;
  margin-bottom: 20px;
  font-weight: bolder;
}
}
</style>
