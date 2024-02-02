<template>
<header>
 <h1 v-on:click="changeTitle">
  {{ titledProp }}
 </h1>

</header>

</template>

<script>

export default {
props:{
  titledProp:{
    type:String
  }
},
  data () {
    return {
title: "This the title"
    }
  },
  methods:{
    changeTitle(){
      this.titledProp = "changed Bottle Title"
    }
  }
  }


</script>

<style scoped>
header{
  background-color: beige;
  padding: 10px;
}
h1{
  color:blueviolet;
  text-align: center;
}
</style>
