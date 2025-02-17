<template>
    <h2>Coche - Composition API</h2>
    <p>Marca: {{ brand }}</p>
    <p>Modelo: {{ model }}</p>
    <p>Potencia: {{ power }} </p>
    <button @click="upPower" > Subir Potencia</button>
    <button>Disminuir</button>
</template>

<script>

export default {
    props: {
        power: {
            type: Number,
            default: 40,
        },

        upPower: Function,
        
    },
    emits:["downPower"],


    setup(props, context) {
        const brand = 'Ford';
        const model = 'Mustang';

        console.log(context);
        

        return {
            brand,
            model,
            
        };
            
    },
};


</script>

<style lang="scss" scoped></style>