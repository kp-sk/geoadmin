<template>
<section>
   <form @submit.prevent="onSubmit">
      <b-field label="Username">
        <b-input type="text" v-model="username" maxlength="255" style="width:300px" required > </b-input>
      </b-field>
      <b-field label="Password">
        <b-input type="password" v-model="password" minlength="6" style="width:300px" password-reveal required ></b-input>
      </b-field>
      <span v-if="error != null">{{error}}</span>
      <b-button native-type="submit" type="is-primary">Login</b-button>
    </form>
</section>
</template>

<script>

export default {
  
  data() {
    return {
      username: "",
      password: "",
      error: null
    };
  },
  methods: {
    onSubmit() {
      var request = {
      
        username:this.username,
        password:this.password
      };
      if(this.username === "abc"){
        this.$router.push("/menu");
      }
      console.log(request)
    }
  }
};
</script>