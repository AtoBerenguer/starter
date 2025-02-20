<template>
    <div>
       
        <h1 id="titulo">Listado de Tareas</h1>
        <hr>
        <div class="row">
            <div class="col">
                <div div class="card">
                    <div class="card-body">
                        <input type="text" class="form-control" placeholder="Ingrese una tarea">
                        <button @click="agregarTarea()" class="btnAgregar">Agregar</button>
                    </div>
                    <div class="listaTareas">
                        <ul class="list-group">

                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "Tarea",
        
        methods:{
            agregarTarea(){
                console.log("Agregando tarea");
            }
        }
        
    }
</script>

<style scoped>
    #titulo{
        
        text-align: center;
        margin-top: 1rem;
        
    }

    .row{
        border: 1px solid black;
        max-width: 66%;
        text-align: center;
        margin: 0 auto;
        display: flex;
        justify-content: center;
        
    }
    .btnAgregar{
    background-color: greenyellow;
    font-size: 1rem;
    border-radius: 15%;    
    }

</style>