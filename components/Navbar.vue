<template>
  <div>
    <b-navbar toggleable="lg" type="dark" variant="dark">
      <div>
        <!-- Just an image -->
        <b-navbar variant="faded" type="light">
          <b-navbar-brand to="/">
            <img class="logoresize" src="~/assets/MuktiLogo.jpg" alt="Mukti" />
          </b-navbar-brand>
        </b-navbar>
      </div>
      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto myclassone">
          <b-nav-item to="/">Home</b-nav-item>
          <b-nav-item to="/about">About</b-nav-item>
           <b-nav-item to="/services">Services</b-nav-item>
          <b-nav-item to="/contact">Contact</b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<style scoped>
.myclassone {
    margin-right: 50px!important;
}
.logoresize {
    height: 130px!important;
}
.navbar-dark .navbar-nav .nav-link{
      color:#373445!important;
      font-weight: bolder;
      margin-right: 25px!important;
      font-size: 22px!important;
    }
.navbar.navbar-dark.bg-dark {
  background-color: #bfd9d6 !important;
  
}
</style>
