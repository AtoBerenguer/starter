<template>
  <h1>Vue Js</h1>
  <CarOptions/> 
  <hr/>
  <CarComposition></CarComposition>
  <div>

  </div>
</template>

<script>
import CarComposition from './components/CarComposition.vue'
import CarOptions from './components/CarOptions.vue'
  export default {
    components: {
      CarComposition,
      CarOptions
    }
  }
</script>

<style lang="scss" scoped>

</style>