<template>
  <div>
    <!-- <h1>Hello from home component</h1> -->
    <!-- <h1 v-if="show">Conditional Rendering</h1> -->
    <h1>For loop in vue.js</h1>
    <table border="1px">
        <tr>
            <td>Id</td>
            <td>Name</td>
            <td>Email</td>
        </tr>

        <tr v-for="user in users" :key="user.id">
            <td>{{user.id}}</td>
            <td>{{user.name}}</td>
            <td>{{user.email}}</td>
        </tr>

    </table>
    <!-- <h1 v-else>else side</h1> -->
    <!-- <button v-on:click="display">Toggle</button> -->
    <!-- <h1>{{ data }}</h1>
    <h1>{{ msg }}</h1> -->

    <!-- <button v-on:mouseover ="hello('data')">Call Hello functiomn</button> -->

  </div>
</template>

<script>
export default {
    name:'HomeView' ,
    props:{
        data:String,
        msg:String
    },
    // methods: {
    //     hello(item) {
    //         console.log(item)
    //     }
    // }
    data(){
        return{
           users: [
                {id:1, name:'Gimhan', email:'gimhan@gmail.com'},
                {id:2, name:'Pabasara', email:'pabasara@gmail.com'},
                {id:3, name:'Munasinghe', email:'munasinghe@gmail.com'},
                {id:4, name:'Wasudewa', email:'wasudewa@gmail.com'},

            ]
        }
    },
    // methods:{
    //     display(){
    //         this.show=!this.show
    //     }
    // }
}
</script>

<style>

</style>