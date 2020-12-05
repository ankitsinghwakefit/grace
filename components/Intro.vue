<template>
  <div class="introContainer">
    <div class="introChild">
     <div>
            <img class="logoresize" src="~/assets/MuktiLogo.jpg" alt="Kitten" />
     </div>
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
    </div>
  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Lobster&display=swap');

.introContainer {
  width: 100%;
  height: 20vh;
  margin: 40px 0;
}
.introChild {
  width: 80%;
  margin: 0 auto;
  display: flex;
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
@media only screen and (max-width: 600px) { 
    .introChild {
  width: 80%;
  margin: 0 auto;
  display: flex;
  flex-direction: column;
}
}
</style>
