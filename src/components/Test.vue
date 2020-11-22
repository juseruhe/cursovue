<template>
<div class="text">
{{msg}}
</div>
</template>

<script>
export default {
    data(){

        return{

            title: "Hola VueJS",

            user:{
          
          firstName: "Juan",
          lastName: "Ruiz"

            },

            myHtml: "<h3>Hola Vue</h3>",

            showName: false,

            tasks:[
              {title: 'eat'},
              {title: 'dinner'},
                {title: 'play'},
              {title: 'taks'}


            ]

        }
    },
methods: {

saludar(firstName) {

    alert("Hello "+firstName);
},

typedEnter(){

console.log('Dio un Enter');



}


    
},
computed: {

    fullName(){

        return this.user.firstName+" "+this.user.lastName;
    }
},

props: {

msg: {

    type: String,

    default: "Mensaje por defecto"

}

}

}
</script>



<style scoped>

.text{

    background:gray;
}

</style>