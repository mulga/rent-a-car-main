<template>
  <div class="d-flex flex-column h-100">
     

    <!-- FOOTER -->
    <footer class="w-100 py-2 flex-shrink-1">
      <div class="container py-1">
        <div class="row gy-4 gx-5">
          <div class="col-lg-4 col-md-6">
            <h5 class="h1 text-white">ERBA</h5>
            <p class="small text-muted">
               
            </p>
            <p class="small text-muted mb-0">
              <a class="text-primary" href="#">&#128231; Erba.com</a> </p>
            <hr>
             <p class="text-white">&copy; Copyrights. All rights reserved.</p> 
              
           
          </div>
          <div class="col-lg-2 col-md-6">
            <h5 class="text-white mb-3">Quick links</h5>
            <ul class="list-unstyled text-muted">
              <li><a href="#">Home</a></li>
              <li><a href="#">About</a></li>
              <li><a href="#">Get started</a></li>
              <li><a href="#">FAQ</a></li>
            </ul>
          </div>
          <div class="col-lg-2 col-md-6">
            <h5 class="text-white mb-3">Social-media</h5>
          <a href="#" class="d-flex align-items-center justify-content-center"
            ><span class="fa fa-facebook"
              ><i class="sr-only">Facebook</i></span
            ></a
          >
          <a href="#" class="d-flex align-items-center justify-content-center"
            ><span class="fa fa-twitter"
              ><i class="sr-only">Twitter</i></span
            ></a
          >
          <a href="#" class="d-flex align-items-center justify-content-center"
            ><span class="fa fa-instagram"
              ><i class="sr-only">Instagram</i></span
            ></a
          >
          <a href="#" class="d-flex align-items-center justify-content-center"
            ><span class="fa fa-dribbble"
              ><i class="sr-only">Dribbble</i></span
            ></a
          >
         
          </div>
          <div class="col-lg-4 col-md-6">
            <h5 class="text-white mb-3">Newsletter</h5>
            <p class="small text-muted">
              Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do
              eiusmod tempor incididunt.
            </p>
            <form action="#">
              <div class="input-group mb-3">
                <input
                  class="form-control"
                  type="text"
                  placeholder="Recipient's username"
                  aria-label="Recipient's username"
                  aria-describedby="button-addon2"
                />
                <button
                  class="btn btn-primary"
                  id="button-addon2"
                  type="button"
                >
                  <i class="fas fa-paper-plane"></i>
                </button>
              </div>
            </form>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  // eslint-disable-next-line 
  name: "Footer",
  components: {},
};
</script>
<style scoped>
body {
  background: #2a2e32;
}

.text-small {
  font-size: 0.9rem;
}

a {
  color: inherit;
  text-decoration: none;
  transition: all 0.3s;
}

a:hover,
a:focus {
  text-decoration: none;
}

.form-control {
  background: #212529;
  border-color: #545454;
}

.form-control:focus {
  background: #212529;
}

footer {
  background: #212529;
}
</style>
