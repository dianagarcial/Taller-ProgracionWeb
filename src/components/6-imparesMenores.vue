<template>
<div id="aplicacion">
    <h1>6. Lista de numeros impares menores</h1>
    <input type="number" v-model="numero">
    <h2 v-if="numero==''">Ingrese el numero para descubrir los impares menores</h2>
    <h2 v-else>{{compara}}</h2>
    
    </div>
    </template>


<script >
export default {
  
      name:'imparMenores',
      data(){
        return{      
          numero:'',
      
        }
      },
      computed: {
        compara(){
            
            let x = 1;
            let n= this.numero;
            let res=[];

            while( x <= n){
                if (x % 2){
                   res.push(x);
                }
                x=x+1;

            }
            return res;           
            

        }
      }
}
</script>