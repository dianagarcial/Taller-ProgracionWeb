<template>
<div id="aplicacion">
    <h1>4. Compara tres numeros</h1>
    <div id="tres">
    <input type="number" v-model="primero">
    <input type="number" v-model="segundo">
    <input type="number" v-model="tercero">
    </div>
    <h2 v-if="primero=='' || segundo==''|| tercero==''">Ingrese los tres numeros a comparar</h2>
    <h2 v-else-if="primero===segundo && segundo ==tercero">Existen 3 numeros iguales</h2>
    <h2 v-else-if="primero===segundo || primero===tercero || segundo===tercero">Existen 2 numeros iguales</h2>
    <h2 v-else>No existen numeros iguales</h2>
    </div>
    </template>


<script >
export default {
  
      name:'tresnumeros',
      data(){
        return{
      
      primero:'',
      segundo:'',
      tercero:''
        }
      
      
      }
    
  
  
}
</script>