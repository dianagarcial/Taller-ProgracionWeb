<template>
<div id="aplicacion">
    <h1>5. Lista de numeros ordenada</h1>
    <div id="res-list">
    <input type="number" v-model="numeroan">
    <button @click="guardar()">Añadir</button>
    </div>
    <h2 v-if="arr.length==0"></h2>
    <h2 v-else>{{arr.sort()}}</h2>

    </div>
    </template>


<script >
export default {
  
      name:'ListaNumeros',
      data(){
        return{
      
      numeroan:'',
      arr:[]
      
        }
        
      },
      methods:{
        guardar(){
            var numeros = this.numeroan;
            this.arr.push(numeros);
            this.numeroan ="";
        }
            
        }
      
}
</script>