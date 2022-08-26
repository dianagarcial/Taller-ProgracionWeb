<template>
<div id="aplicacion">
  <h1>12. Calculo notas con arreglos</h1>
    <h1>Ingrese su nombre</h1>
    <input type="text" v-model="estudiante[0]">
    <h1>Ingrese sus notas</h1>
    <div id="res">
    <input type="number" v-model="estudiante[1]" >
    <input type="number" v-model="estudiante[2]">
    <input type="number" v-model="estudiante[3]">
    
    
    
   
   </div>

   <h2 v-if="estudiante[0]===''||estudiante[1]===''||estudiante[2]===''||estudiante[3]===''"></h2>
    <h2 v-else>Hola {{estudiante[0]}},en esta ocasion usted {{notas}} la materia</h2>
    
   
    </div>
    </template>


<script >


export default {
  
      name:'ArrNotas',
      data(){
        return{
            estudiante:[4]
      
      
      
        }

        
      },
      computed:{
        notas(){
            var prom=0;
            prom=Number((this.estudiante[1]+this.estudiante[2]+this.estudiante[3]))/3
            
            if(prom >= 3.0){
                
                return 'pasa'


            }else{
                return 'no pasa'
            }
            
          }
            
        }
            
        
        
            
        }
      

</script>