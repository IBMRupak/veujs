<template>
    <div>

        <h1>Data Bind</h1>


<!-- One way Data Binding -->
        <h1 style="white-space:pre-line">{{message}}</h1> 
         <!-- view part --> 
         <!-- Data binding -->
      <!-- <input type= "text" v-model="message">            -->

      <textarea type="text" v-model="message"/>

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