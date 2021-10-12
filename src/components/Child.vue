 <template>
     <div>
         <h1>Child Component</h1>
        <tr v-for="user in users" :key="user.name">
             {{user.name}} -- {{user.email}}
        </tr>
         </div>

 </template>

<script>
export default {
    name: 'Child',
    props:['users']
}
</script>