<template>
  <Auth>
    <form class="form-signin" @submit.prevent="myDataSend">
      <h1 class="h3 mb-3 font-weight-normal">Sign Up</h1>
      <label for="fullName" class="sr-only">Full Name</label>
      <input
        type="text"
        id="fullName"
        class="form-control"
        placeholder="Full name"
        v-model="user.fullName"
         
      />
      <label for="inputEmail" class="sr-only">Email address</label>
      <input
        type="email"
        id="inputEmail"
        class="form-control"
        placeholder="Email address"
        v-model="user.email"
         
      />

      <label for="inputPassword" class="sr-only">Password</label>
      <input
        type="password"
        id="inputPassword"
        class="form-control"
        placeholder="Password"
        v-model="user.password"
      />

      <label for="inputPasswordConfirm" class="sr-only"
        >Password Confirmation</label
      >
      <input
        type="password"
        id="inputPasswordConfirm"
        class="form-control"
        placeholder="inputPasswordConfirm"
        v-model="user.password_confirmation"
      />

      <button class="btn btn-lg btn-primary btn-block" type="submit">
        Sign Up
      </button>
      <p class="mt-5 mb-3 text-muted">&copy; 2017-2022</p>
    </form>
  </Auth>
</template>

<script>
 
 
import Auth from "@/components/Auth.vue";

export default {
  // eslint-disable-next-line
  name: "Register",

  components: {
    Auth,
  },
   
  data() {
    return {
      user: {
        fullName: null,
        email: null,
        password: null,
        password_confirmation: null,
      },
    };
  },
  methods: {
    myDataSend() {
       
      fetch(
        "https://mini-garten-default-rtdb.europe-west1.firebasedatabase.app/umfrage.json",
        {
          method: "POST",
          headers: {
            "Content-Type": "application/json",
          },
          body: JSON.stringify({
            username: this.fullName,
            password: this.password,
            password_confirmation: this.password_confirmation,
          }),
        }
      );
    },
  },
  
}
</script>

<style></style>
