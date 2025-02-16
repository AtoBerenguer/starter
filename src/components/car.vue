<template>
    <h2>Coche - Composition API</h2>
    <p>Marca: {{ brand }}</p>
    <p>Modelo: {{ model }}</p>
    <p>Potencia: {{ power }} </p>
</template>

<script>

export default {
    props: {
        power: {
            type: Number,
            default: 40,
        },
    },
    setup(props) {
        const brand = 'Ford';
        const model = 'Mustang';
        console.log(props);
        
      
        
        return {
            brand,
            model,
        };
            
    },
};


</script>

<style lang="scss" scoped></style>