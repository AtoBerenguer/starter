<template>
    <h2>Coche - Composition API</h2>
    <p>Marca: {{ brand }}</p>
    <p>Modelo: {{ model }}</p>
    <p>Potencia: {{ power }}</p>
    <button @click="upPower">Aumentar CV</button>
    
    <button @click="downPower">Disminuir CV</button>
</template>

<script >
import { ref } from 'vue';
export default {
    setup(){
        const brand = 'Ford';
        const model = 'Mustang';
        let power = ref(40);

        const upPower = () => {
            console.log("Aumentado potencia");
            console.log(power.value);
            power.value ++;         
        };
        const downPower = () => {
            console.log("Disminuir potencia ");
            power.value --;
        };
        return {
            brand,
            model,
            power,
            upPower,
            downPower,
        };
    },
};
    

</script>

<style lang="scss" scoped>

</style>