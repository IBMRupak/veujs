<template>
  <div>
    <input type="text" placeholder="Enter your name" v-model="signup.username"/><br /><br />
    <input type="password" placeholder="Enter your password" v-model="signup.password" /><br /><br />
    <p>Choose Hobbies</p>
    <input type="checkbox" id="cricket" value="cricket" v-model="signup.hobbies" />
    <label for="cricket">Cricket </label>
    <input type="checkbox" id="fotball" value="fotball" v-model="signup.hobbies" />
    <label for="fotball">Football </label>
    <br />
    <br />
    <p>Select Gender</p>
    <input type="radio" id="male" value="male" v-model="signup.gender"/>
    <label for="male">MAle</label>
    <input type="radio" id="female" value="female" v-model="signup.gender" />
    <label for="female">FeMAle</label>
    <br /><br />
    <button v-on:click="signupUser">Sign Up</button>
  </div>
</template>

<script>
export default {
    name:'SignUp',
    data()
    {
        return{
            signup:{
                username:null,
                password:null,
                hobbies:[],
                gender:null
            }
        }
    },
    methods:{
        signupUser()
        {
        console.warn(this.signup)
        }
    }
}
</script>