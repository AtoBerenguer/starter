<template>
    <h2>Coche - Options API</h2>
    <p>Marca: {{ brand }}</p>
    <p>Modelo: {{ model }}</p>
    <p>Potencia: {{ power }}</p>
    <button @click="upPower(50)">Aumentar CV</button>
    <button @click="downPower">Disminuir CV</button>
</template>

<script >
export default {
    data(){
        return{
            brand: 'Seat',
            model: 'Leon',
            power: 50,
        }
    },

    methods: {
        upPower(newPower){
            
            this.power += newPower;
            
        },
        downPower(){
            console.log("Disminuir potencia");
            this.power -= 10;
        },
    },
};
    

</script>

<style lang="scss" scoped>

</style>