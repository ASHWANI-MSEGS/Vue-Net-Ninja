<template>
  <div>
<app-header v-bind:titledProp="titled"></app-header>
<!-- here ninJas(is the prop name in ninjas file and "ninja" is the data we pass from the data below) -->
<app-ninja v-bind:ninJas="ninjas"></app-ninja>


<app-footer v-bind:titledProp="titled" ></app-footer>
</div>
</template>

<script>
import header from './components/Header.vue'
import footer from './components/Footer.vue'
import ninja from './components/Ninjas.vue'
export default {

  components: {
    "app-header":header,
    "app-footer":footer,
    "app-ninja":ninja
  },
  data () {
    return {
      ninjas: [
                {name: 'Ryu', speciality: 'Vue Components', show: false},
                {name: 'Crystal', speciality: 'HTML Wizardry', show: false},
                {name: 'Hitoshi', speciality: 'Click Events', show: false},
                {name: 'Tango', speciality: 'Conditionals', show: false},
                {name: 'Kami', speciality: 'Webpack', show: false},
                {name: 'Yoshi', speciality: 'Data Diggin', show: false}
            ],
        titled: "Bottle TITLE",
    }
  }
  }


</script>

<style >


</style>
