<template>
  <section class="container">
    <h1>{{title}}</h1>
    <form>
        <div class="form-group">
            <label for="exampleInputEmail1">Email address</label>
            <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" placeholder="Enter email" v-model= "email">
            <small id="emailHelp" class="form-text text-muted">We'll never share your email with anyone else.</small>
        </div>
        <div class="form-group">
            <label for="exampleInputPassword1">Password</label>
            <input type="password" class="form-control" id="exampleInputPassword1" placeholder="Password" v-model= "password">
        </div>
        <div class="form-check">
            <input type="checkbox" class="form-check-input" id="exampleCheck1" v-model= "checkMeOut">
            <label class="form-check-label" for="exampleCheck1">Check me out</label>
        </div>
        <button @click.prevent= "onSubmit" type="button" class="btn btn-primary">Submit</button>
        </form>
  </section>
</template>

<script>
import AppLogo from '~/components/AppLogo.vue'

export default {
  components: {
    AppLogo
  },
  data(){
      return {
          title: 'Sample title',
          email: '',
          password: '',
          checkMeOut: false
      }
  },
  methods: {
      onSubmit() {
          //jQuery way
          // let test = jQuery('#exampleInputEmail1').val();

          //vue way
          let email = this.email;
          let password = this.password;
          let checkMeOut = this.checkMeOut;
      }
  }
}
</script>