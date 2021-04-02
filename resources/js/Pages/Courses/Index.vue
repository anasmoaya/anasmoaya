<template>
<app-layout>
   <template #header> <h1>this is cool</h1>
   <dropdown-link>XXXXXXXXX</dropdown-link>
   </template>
   <div v-for="cours in Courseliste "  v-bind:key="cours.id" >
       <table>
           <tr ></tr>
       </table>
       <div>{{cours.title}}</div>
       <div>{{cours.description}}</div>
       
   </div>
</app-layout>

     
    
</template>
<script>
import NavLink from '../../Components/NavLink.vue'
import AppLayout from '../../Layouts/AppLayout.vue'
import Welcome from '../Welcome.vue'
import DropdownLink from '../../Components/DropdownLink'



export default {
    components:{
        AppLayout,
        NavLink,
        Welcome,
        DropdownLink,
    
    },
        data(){
        return {Courseliste : this.tutos}
    },

    props:['tutos'],
      
    }

  

        
    

</script>