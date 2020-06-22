<template>
  <div>
    <b-container fluid>
      <h1>Login</h1>
      <UserAuthForm buttonText="Login" :submitForm="loginUser" />
    </b-container>
  </div>
</template>

<script>
import UserAuthForm from '@/components/login/UserAuthForm'
export default {
  components: {
    UserAuthForm
  },
   methods: {
    async loginUser(loginInfo) {
        //alert(loginInfo);
      try {
        let response = await this.$auth.loginWith('google', { data: loginInfo })
        console.log(response)
      } catch (err) {
        console.log(err)
      }
    }
  }

//   methods: {
//     loginUser(loginInfo) {
//       // debugger
//       //alert(JSON.stringify(this.form))
//       this.$auth.loginWith('local', {
//         data: loginInfo
//       })
//     }
//   }
}
</script>

<style>
</style>