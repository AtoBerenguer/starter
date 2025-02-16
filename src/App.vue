<template>
  <h1>Vue Js</h1>
   
  
  <car :power="power" />
  <div>

  </div>
</template>

<script>
import car from './components/car.vue'
  export default {
    components: {
      car,
      
    },
    setup() {
      let power = 39;

      return{
        power,
      };

    }
  }
</script>

<style lang="scss" scoped>

</style>