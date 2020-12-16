<template>
  <div class="introcontainer">
    <b-container>
      <b-row>
        <b-col xl="6" lg="6" md="6" sm="12">
          <div>
            <img class="logoresize" src="~/assets/MuktiLogo.jpg" alt="Mukti" />
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
             <li>
                 We Welcome you to Devbhumi - Himachal Pradesh to get Mukti.
             </li>
         </ul>
         </div>
        </b-col>
      </b-row>
    </b-container>
  </div>
 
</template>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Lobster&display=swap");


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
