<template>
  <footer>
 <p>

    {{footer}} {{ titledProp }}

 </p>

  </footer>

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
  footer: "This the copyright of "
      }
    }
    }


  </script>

  <style scoped>
  footer{
    background-color:rgb(204, 135, 31);
    padding: 10px;
  }
  p{
    color:rgb(43, 61, 226);
    text-align:left;
  }
  </style>
