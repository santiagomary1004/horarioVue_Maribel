<script>
    export default {
        data(){
            return{
                //DATOS DE ALUMNOS
                alumnos:[
                    {nc:12345, nombre: 'Maribel', carrera:'ISC'},
                    {nc:12345, nombre: 'Natalia', carrera:'TICS'},
                    {nc:12345, nombre: 'Carlos', carrera:'ISC'},
                    {nc:12345, nombre: 'Rodrigo', carrera:'TICS'},

                ]
            }
        }
    }
</script>

<template>
<div class="container">
    <h3 class="mt-4">Lista de alumnos</h3>
    <ul>
        <li v-for="alumno in alumnos" :key="alumno.nc">
            <strong>{{ alumno.nombre }} </strong> -
            <strong>{{ alumno.carrera }} </strong>

        </li>
    </ul>
</div>
</template>
<style scoped>
h3{
    color:white;
    background-color: rgb(205, 132, 239);
    border-radius: 15px;
    padding: 10px;
    text-align: center;
}
ul{
    list-style-type: none;
    padding: 0px;
}
li{
    color:white;
    background-color: black;
    border-radius: 15px;
    padding:10px;
    margin: 10px;
    text-align:justify;
}
</style>