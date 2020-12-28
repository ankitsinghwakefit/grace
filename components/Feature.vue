<template>

  <div class="featurecontainer">
   
    <b-container class="">
      
      <b-row>
        <div class="featureheading">
          Features
        </div>
      </b-row>

      <b-row>
        <b-col xl="6" lg="6" md="6" sm="12">
          <div class="mt-3">
            <b-card-group deck class="mb-3">
              <b-card
                border-variant="dark"
                header="Location"
                class="text-center"
              >
                <b-card-text>
                  <span class="home">CITY</span>, a small Village - Kangra (Away from
                  cities) in Heart of Dharamshala - Himachal Pradesh.
                </b-card-text>
              </b-card>
            </b-card-group>
          </div>
        </b-col>
        <b-col xl="6" lg="6" md="6" sm="12">
          <div class="mt-3">
            <b-card-group deck class="mb-3">
              <b-card
                border-variant="dark"
                header="Pick up drop off service"
                class="text-center"
              >
                <b-card-text
                  >Airport/Bus stand pick up or drop off service to avoid any Inconvenience.</b-card-text
                >
              </b-card>
            </b-card-group>
          </div>
        </b-col>
      </b-row>
      <!-- <b-row>
        <b-col xl="6" lg="6" md="6" sm="12">
          <div class="mt-3">
            <b-card-group deck class="mb-3">
              <b-card
                border-variant="dark"
                header="SightSeeings"
                class="text-center"
              >
                <b-card-text
                  >The spectacular Kangra Valley is famous for its magical charm
                  and spellbound beauties, lush green surroundings, revered
                  goddess temples & famous Kangra Tea Bagan.</b-card-text
                >
              </b-card>
            </b-card-group>
          </div>
        </b-col>
        <b-col xl="6" lg="6" md="6" sm="12">
          <div class="mt-3">
            <b-card-group deck class="mb-3">
              <b-card
                border-variant="dark"
                header="Connectivity"
                class="text-center"
              >
                <b-card-text
                  >Kangra can be reached by Bus, Train & Flight as well -
                  Gaggal-Kangra Airport is open all year round!</b-card-text
                >
              </b-card>
            </b-card-group>
          </div>
        </b-col>
      </b-row> -->
      <b-row>
        <b-col xl="6" lg="6" md="6" sm="12">
          <div class="mt-3">
            <b-card-group deck class="mb-3">
              <b-card
                border-variant="dark"
                header="Fun on demand"
                class="text-center"
              >
                <b-card-text
                  ><span class="fun">Paragliding</span> - Over high mountains in the region.<br>
                  <span class="fun">Trekking</span> - Himachal is a playground for trekkers.<br>
                  <span class="fun">Camping</span> - The best way to enjoy the wonders of nature.<br>
                  
                </b-card-text>
              </b-card>
            </b-card-group>
          </div>
        </b-col>
        <b-col xl="6" lg="6" md="6" sm="12">
          <div class="mt-3">
            <b-card-group deck class="mb-3">
              <b-card
                border-variant="dark"
                header="Accommodation"
                class="text-center"
              >
                <b-card-text>High-Speed Internet.<br>
                Comfortable Stay.<br>
               Table - Chair & Work Desks to WFH(Himachal).<br>
                Tea, Breakfast, Lunch & Dinner.<br></b-card-text>
              </b-card>
            </b-card-group>
          </div>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Andika+New+Basic:ital,wght@0,400;0,700;1,400;1,700&display=swap');
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
  background-color: #658EA9;
  color: #373445;
  font-size: 25px;
  font-weight: bolder;
}
.featurecontainer {
   background-color: #E7D4C0;
  padding-bottom: 50px;
  font-family: 'Andika New Basic', sans-serif;
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
</style>
