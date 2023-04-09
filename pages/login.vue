<template>
    <div class="d-flex ">
        <div class="image-container">
            <img class="" alt="Login image" src="@/assets/fleet-login.png">
        </div>
        <div class="login-container">
          <div>
            <v-container class="login-wrapper">
                <v-form @submit.prevent="login">
                <v-text-field v-model="email" label="Email"></v-text-field>
                <v-text-field v-model="password" label="Password" type="password"></v-text-field>
                <v-btn type="submit" color="primary">Sing In</v-btn>
                </v-form>
            </v-container>
          </div>
        </div>
    </div>
  </template>
  
  <script>  
  export default {
    layout: 'loginlayout',
    data() {
      return {
        email: '',
        password: '',
      };
    },
    methods: {
      login() {
        // Call your authentication API endpoint with email and password
      },
    },
  };
  </script>
  <style>
/* Style for the image container */
.image-container {
  /* width: 50%;
  height: 100%;
  float: left; */
}

/* Style for the login container */
/* .login-container {
  width: 50%;
  height: 100%;
  float: right;
  display: flex;
  justify-content: center;
  align-items: center;
} */

/* Style for the image inside the image container */
/* .image-container img {
  width: 100%;
  height: 80%;
  object-fit: cover;
} */
/* .login-wrapper{

} */
  </style>
  