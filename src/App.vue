<template>
  <h1>Vue Js</h1>
   
  
  <car :power="power" :upPower="upPower" @downPower="downPower" />
  <div>

  </div>
</template>

<script>
import { ref } from 'vue';
import car from './components/car.vue'
  export default {
    components: {
      car,
      
    },
    setup() {
      let power = ref(39);

      const upPower = () => {
        power.value ++;
        
      };

      const downPower = () => {
        power.value --;
      };

      return{
        power,
        upPower,
        downPower,
      };

    }
  }
</script>

<style lang="scss" scoped>

</style>