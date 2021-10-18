<template>
    <div>
        <input type="text" placeholder="enter Username" name="username" v-model="LoginForm.username"/><br><br>
         <input type="password" placeholder="enter password" name="password" v-model="LoginForm.password"/><br><br>
         <button v-on:click="loginData">Login</button>
    </div>
</template>
<script>
export default {
    name:'Login',
    methods:{
        loginData(){
            console.log("Login Data",this.LoginForm)

        }
    },
    data()

    {
        return{
      LoginForm:{
          username:null,
          password:null
      }
        } 
    }
}
</script>