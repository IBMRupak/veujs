<template>
    <div>

        <h1>Data Bind</h1>

        <h1>{{message}}</h1> 
         <!-- view part --> 
         <!-- Data binding -->
      <input type= "text" v-model="message">           

    </div>
</template>

<script>
export default {
    name: 'DataBind',
    data(){
        return{
            message:"Hi"            //model part
        }
    }
}
</script>