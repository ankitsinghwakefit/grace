<template>
  <div class="heroImg">
    <div class="heroPic">
    <!-- <vue-typer type='Array' text='Hello World! I was registered locally!'></vue-typer> -->
    <p> Weather you are : <vue-typer class="mytyper"
  :text='["Tourist","A Nature lover","Employee","Businessman","Pilgrim"]'
  :repeat='Infinity'
  :shuffle='false'
  initial-action='typing'
  :pre-type-delay='70'
  :type-delay='70'
  :pre-erase-delay='2000'
  :erase-delay='250'
  erase-style='select-all'
  :erase-on-complete='false'
  caret-animation='blink'
></vue-typer></p>
      
      <h3> ~ let's escape this town for a little while ~ </h3>
      <!-- <button>Let's Get IT!</button> -->
      <b-link to="/contact" class="button" style="vertical-align:middle"><span>Chalo, Let's Go!</span></b-link>
      </div>
  </div>
</template>


<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Lobster&display=swap');
.button {
  display: inline-block;
  border-radius: 13px;
  /* background-color: #FFA384; */
  box-shadow: 0px 4px 0px 0px rgba(0,0,0,0.75);
  border: 1px groove #373445;
  color: #373445;
  text-align: center;
  font-size: 28px;
  padding: 15px;
  width: 280px;
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
h1 {
    font-size: 100px;
    font-weight: bolder;
    color: #373445;
}
h3 {
    font-size: 50px;
    color: #373445;
    font-family: 'Lobster', cursive;
}
.heroImg {
    width: 100%;
    height: 63vh;
    /* background-color: #FFA384; */
    /* display: flex;
    flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center; */
}
.heroPic {
  background-image: url("~assets/heroImg.jpg");
  background-repeat: no-repeat;
  width: 100%;
  height: 100%;
  background-position: center;
    background-size: cover;
    display: flex;
    flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}
p {
  font-size: 30px;
  color: #373445;
}

.vue-typer .custom.char {
  color: #D4D4BD;
  background-color: #1E1E1E;
}
.vue-typer .custom.char.selected {
  background-color: #264F78;
}

.vue-typer .custom.caret {
  width: 10px;
  background-color: #3F51B5;
}
@media only screen and (max-width: 900px) {
  .button {
  display: inline-block;
  border-radius: 13px;
  box-shadow: 0px 4px 0px 0px rgba(0,0,0,0.75);
  /* border: 1px dotted #373445; */
  
  color: #373445;
  text-align: center;
  font-size: 28px;
  padding: 20px;
  width: 290px;
  transition: all 0.5s;
  font-weight: bolder;
  cursor: pointer;
  margin: 5px;
}
h1 {
    font-size: 80px;
    font-weight: bolder;
    color: #373445;
}
h3 {
    font-size: 40px;
   color: #373445;
    font-family: 'Lobster', cursive;
}
.heroImg {
    width: 100%;
    height: 58vh;
    background-color: #373445;
    display: flex;
    flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}
p {
  font-size: 25px;
  color: #373445;
}
}
@media only screen and (max-width: 786px) {
  p {
  font-size: 20px;
  color: #373445;
}
}
@media only screen and (max-width: 350px) {
  .button {
  display: inline-block;
  border-radius: 13px;
  box-shadow: 0px 4px 0px 0px rgba(0,0,0,0.75);
  border: 1px groove #373445;
  
  color: #373445;
  text-align: center;
  font-size: 25px;
  padding: 20px;
  width: 270px;
  transition: all 0.5s;
  font-weight: bolder;
  cursor: pointer;
  margin: 4px;
}
h1 {
    font-size: 65px;
    font-weight: bolder;
    color: #373445;
}
h3 {
    font-size: 30px;
    color: #373445;
    font-family: 'Lobster', cursive;
}
.heroImg {
    width: 100%;
    height: 63vh;
    background-color: #373445;
    display: flex;
    flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}
p {
  font-size: 20px;
  color: #373445;
}
}

</style>
