<template>
    <div>
        <h2>Coche</h2>
        <p>Marca: {{brand}}</p>
        <p>Modelo: {{model}}</p>
        <p>Potencias:</p>
        <ul>
            <template v-for="(power,index) in powers " :key="index" >
                <li v-if="power < 240">Urbana:{{power}} CV</li>
                <li v-else-if="power === 250">Hibrida:{{power}} CV</li>
                <li v-else>Carrera: {{ power }} CV</li>
            </template>
        </ul>
        
    </div>
</template>

<script>
export default {
   
    setup() {
        const brand = 'Ford';
        const model = 'Mustang';
        const powers = [60,100,150,200,250,300,350,500,600,700];
        
        
        return {
            brand,
            model,
            powers,
        };
    }
}
</script>

<style lang="scss" scoped></style>