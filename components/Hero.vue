<template>
  <div class="heroImg">
      <h1>MUKTI</h1>
      <h3> ~ let's escape this town for a little while ~ </h3>
      <!-- <button>Let's Get IT!</button> -->
      <button class="button" style="vertical-align:middle"><span>Let's Get IN!</span></button>
  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Lobster&display=swap');
.button {
  display: inline-block;
  border-radius: 13px;
  background-color: #AB9856;
  border: none;
  color: #373445;
  text-align: center;
  font-size: 28px;
  padding: 20px;
  width: 250px;
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
    color: #AB9856;
}
h3 {
    font-size: 50px;
    color: #AB9856;
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

</style>
