<template>
     
  <nav
    class="navbar navbar-expand-lg ftco_navbar ftco-navbar-light"
    id="ftco-navbar"
  >
    <div class="container">
      <a class="navbar-brand" href="index.html">Erba Rent A Car</a>
      <div class="social-media order-lg-last">
        <div class="row authenticated" v-show="!authShow">
            <div class="test">
              <router-link
                :to="{ name: 'Register' }"
                class="btn btn-warning btn-block"
                >Register</router-link
              >
              <router-link
                :to="{ name: 'Login' }"
                class="btn btn-primary btn-block"
                >Login</router-link
              >
            </div>
          </div>
      </div>
      <button
        class="navbar-toggler"
        type="button"
        data-toggle="collapse"
        data-target="#ftco-nav"
        aria-controls="ftco-nav"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="fa fa-bars"></span> Menu
      </button>
      <div class="collapse navbar-collapse" id="ftco-nav">
        <ul class="navbar-nav ml-auto mr-md-3">
          <li class="nav-item active"><a href="/" class="nav-link">Home</a></li>
          <li class="nav-item"><a href="#" class="nav-link">About</a></li>
          <li class="nav-item"><a href="#" class="nav-link">Work</a></li>
          <li class="nav-item"><a href="#" class="nav-link">Blog</a></li>
          <li class="nav-item"><a href="#" class="nav-link">Contact</a></li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>

export default {
    // eslint-disable-next-line
    name: "Navbar",
}
</script>

<style>

</style>