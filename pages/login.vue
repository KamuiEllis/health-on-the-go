<template>

    <div class="col-3 m-auto" >
          <div class="login-form">
              <card style="margin-top:50%;">
    <h5 slot="header" class="title">Login</h5>
    <form @submit.prevent="updateProfile">
      <div class="row">
        <div class="col-12">
          <base-input
            type="text"
            label="Email"
            placeholder="Email"
            v-model="email"
          >
          </base-input>
        </div>
        <div class="col-12" style="margin-bottom:20px">
          <base-input
            type="password"
            label="Password"
            placeholder="password"
            v-model="password"
          >
          </base-input>
        </div>
        

      <base-button native-type="submit" type="primary" class="btn-fill col-6 m-auto" style='margin-top:5%; margin-bottom:5%;' >
        Save
      </base-button>
      </div>
    </form>
  </card>
          </div>
    </div>


</template>
<script>


import EditProfileForm from '../components/UserProfile/EditProfileForm.vue';

  export default {
    
    layout: 'login',

    components: {
      EditProfileForm
    },
    data() {
      return {
          email: '',
          password: ''
      };
    },

    methods: {
     
    },



  };
</script>
