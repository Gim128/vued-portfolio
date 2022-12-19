<template>
  <div>
    <!-- <h1>Hello from home component</h1> -->
    <h1>Event</h1>
    <!-- <h1>{{ data }}</h1>
    <h1>{{ msg }}</h1> -->

    <button v-on:mouseover ="hello('data')">Call Hello functiomn</button>

  </div>
</template>

<script>
export default {
    name:'HomeView' ,
    props:{
        data:String,
        msg:String
    },
    methods: {
        hello(item) {
            console.log(item)
        }
    }
}
</script>

<style>

</style>