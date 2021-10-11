<template>
  <div>
    <!-- Component in Vue JS -->

    <!-- 
     <h1>This is Rupak</h1> 
    <h2>{{ msg }}</h2>
    <h3>{{data}}</h3> -->

    <!-- Click events in Vue JS -->
    <!-- 
    <button v-on:click = "hello">Click here</button> 
    <br><br>
    <button v-on:mouseover="demo('its demo')"  >demo</button> -->

    <!-- Conditional Rendering -->

    <!-- <h1 v-if="show">Conditional rendering</h1>
    <h1 v-else>Conditional rendering else</h1>
    <button v-on:click="display">Toggle Element</button> -->

    <!-- For loops in Veujs -->

    <!-- <table border="1px" >
      <tr>
        <td>ID</td>
        <td>NAME</td>
        <td>Email</td>
      </tr>
      <tr v-for ="user in users" :key = user.id >
        <td>{{user.id}}</td>
        <td>{{user.name}}</td>
        <td>{{user.email}}</td>
      </tr>

    </table> -->

    <!-- Composing with Components -->

    <h1>Home Component</h1>
    <Users/>
    <Products/>

  </div>
</template>
<script>
import Users from './Users.vue'
import Products from './Products.vue'


export default {
  name: "Home",
  // props: {
  //   msg: String,
  //   data: String,
  // },
  // methods: {
  //   //methods in Vuejs
  //   hello() {
  //     alert("Hey!!!");
  //   },

  //   demo(tim) {
  //     alert(tim);
  //   },
  // },
  // data() {
  //   return{ show:false }
  // },
  // methods : {
  //   display()
  //   {

  //     this.show = !this.show
  //   }
  // }

  // data()
  // {
  //   return{
  //     users : [
        
  //        { id:1, name : 'Ruturaj', email : 'rr@gmail.com'},
  //         {id:2, name : 'FAF', email : 'FAf@gmail.com'},
  //         {id:3, name : 'Uthapa', email : 'uth@gmail.com'},
  //         {id:4, name : 'Dhoni', email : 'msd@gmail.com'}, 
        
  //     ]
  //   }
  // }

  components:{
    Users,
    Products
  }
};
</script>

<style scoped>
div{
  background-color: beige;
  height: 500px;
}
</style>
