<template>
    <div class="users"> 

<h1> User Component</h1>
<ul>
<li v-for="user in users" :key="user.name" >
    
    {{user.name}}

    {{user.email}} 
</li>

<form v-on:submit.prevent="addUser">

<input type="text" v-model="newUser.name" placeholder="nombre">
<input type="email" v-model="newUser.email" placeholder="correo">
<button type="submit"> Add  </button>


</form>


</ul>

    </div>
</template>


<script>
export default {

    data(){

        return{

            users: [
      {
      name: "Juan",

      email: "jsruiz@gmail.com",

      contacted: false

      },

 {
      name: "Sebastian",

      email: "sebasruiz@gmail.com",

      contacted: false

      },

       {
      name: "Luisa",

      email: "luisa@gmail.com",

      contacted: true

      }





            ],

newUser: {}



        }
    }, 

    methods: {

       addUser(){

         

           console.log("Usuario Agregado");
       }

    }
    
}
</script>


<style scoped>

.users{
    background: #333;
    color:white;
}

</style>