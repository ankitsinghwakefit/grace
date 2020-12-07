<template>
  <div class="introcontainer">
    <b-container>
      <b-row>
        <b-col xl="6" lg="6" md="6" sm="12">
          <div>
            <img class="logoresize" src="~/assets/MuktiLogo.jpg" alt="Logo" />
        </div>
          </b-col
        >
        <b-col xl="6" lg="6" md="6" sm="12">
            <div>
            <ul>
             <li>
                 Work From <span class="home">Home</span> Himachal.
             </li>
             <li>
                 Sit by the window when it rains & read book.
             </li>
             <li>
                 Listen to yourself.
             </li>
             <li>
                 Fall asleep when the moon is high & wake up slowly, with no place to rush off to.
             </li>
             <li>
                 Just be boundless & infinite.
             </li>
         </ul>
         </div>
        </b-col>
      </b-row>
    </b-container>
  </div>
  <!-- <div class="introContainer">
    <div class="introChild">
     <div class="intrologobox">
            <img class="logoresize" src="~/assets/MuktiLogo.jpg" alt="Kitten" />
     </div>
     <div class="introlistbox">
         <ul>
             <li>
                 Work From <span class="home">Home</span> Himachal.
             </li>
             <li>
                 Sit by the window when it rains & read book.
             </li>
             <li>
                 Listen to yourself.
             </li>
             <li>
                 Fall asleep when the moon is high & wake up slowly, with no place to rush off to.
             </li>
             <li>
                 Just be boundless & infinite.
             </li>
         </ul>
     </div>
    </div>
  </div> -->
</template>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Lobster&display=swap");

/* .introContainer {
  width: 100%;
  height: 20vh;
  margin: 40px 0;
}
.introChild {
  width: 60%;
  margin: 0 auto;
  display: flex;
}
.intrologobox {
    width: 35%;
}
.introlistbox {
    width: 100%;
}
.other {
    background-color: #AB9856;
}
.introHeading {
    font-family: 'Lobster', cursive;
    color: #AB9856;
    font-size: 30px;
}
ul {
    margin-top: 50px;
}
li {
    font-size: 20px;
    color: #373445;
}
.home {
    text-decoration: line-through;
    color: brown;
}
@media only screen and (max-width: 1100px) { 
    .introChild {
  width: 100%;
  margin: 0 auto;
  display: flex;
  flex-direction: column;
  align-items: center;
}
.intrologobox {
    width: 60%;
}
.logoresize {
    width: 100%;
}
}
@media only screen and (max-width: 800px) { 
    .introChild {
  width: 100%;
  margin: 0 auto;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
.intrologobox {
    width: 100%;
}
.logoresize {
    width: 350px;
}
} */
.introcontainer {
    margin-bottom: 50px;
}
.home {
    text-decoration: line-through;
    color: brown;
}
.logoresize {
    width: 350px;
}
ul {
    margin-top: 50px;
}
li {
    font-size: 20px;
    color: #373445;
}
@media only screen and (max-width: 750px) { 
   ul {
    margin-top: 1px;
}
.introcontainer {
    margin-bottom: 1px;
}
.logoresize {
    width: 310px;
}
}
</style>
