<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <!-- <Home /> -->
    <!-- <Home msg ="Vue JS is awesome" data="Its easy to learn"/> -->
    <!-- <DataBind /> -->
    <!-- <Child  v-bind:users="users"  /> -->
<!-- 
    <h1>{{title}}</h1>
    <ChildToParent v-on:changeTitle="updateTitle($event)"/> -->
    <!-- <h1>Form using checkbox and radio button </h1>
    <SignUp/> -->
<h1>Make form and get data</h1>
<Login/>

  </div>
</template>

<script>
// import Child from './components/Child.vue'
// import HelloWorld from './components/HelloWorld.vue'
// import Home from './components/Home.vue'
// import DataBind from './components/DataBind.vue'
// import ChildToParent from './components/ChildToParent.vue'
// import SignUp from './components/SignUp.vue'
import Login from './components/Login.vue'
export default {
  name: 'App',
  components: {
    // HelloWorld,
    // Home
    // DataBind
    // Child,
    // ChildToParent
   
   Login
    
  },
  // data()
  // {
  //   return { users :[
  //     {
  //       name:"Asif",email :"Abc@gmail.com"
  //     },
  //     {
  //       name:"Akib",email :"Abcd@gmail.com"
  //     },
  //     {
  //       name:"Abid",email :"Abcde@gmail.com"
  //     }
  //   ]
  //   }
  // }

//   data(){
//     return{title:"props tutorial"}
//   },
//   methods:{
//     updateTitle(title)
//     {
//       this.title=title;
//     }
//   }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
