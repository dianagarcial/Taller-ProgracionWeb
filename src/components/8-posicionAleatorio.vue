<template>
<div id="aplicacion">
    <h1>8. Division de numeros aleatorios</h1>
    <div id="res">
    <input type="number" v-model="posicion">
    <button v-on:click.once="generar()">Generar Arreglo</button>
    <button @click="dividir()">Dividir</button>
    
   
   </div>
   
   <h2 id="random"></h2>
   <h2 id="random2"></h2>

    
   
    </div>
    </template>


<script >


export default {
  
      name:'PosicionAleatoria',
      data(){
        return{
      
      posicion: null,
      arr:[],
      arrem:[],
      ver:false
      
        }

        
      },
      methods:{
        dividir(){
          
          
            var numeros = this.posicion;
            
            var array=this.arr;
            var arregloN=this.arrem;
            console.log(array)
            if(this.ver){
            if(numeros >=0 && numeros<=10  ){
          
            for (let index = 0; index < 10; index++) {
              var divisor= array[numeros];
              arregloN.push((array[index]/divisor).toFixed(2));
                     
              
            }
            var body = document.getElementById('random2')
            var textoCelda = document.createTextNode(this.arrem)
            body.appendChild(textoCelda);

            }else if(numeros === null){
               alert('Digite un numero ')
              }else{
              alert('Digite un numero entre 0 y 10')
            }
            }else{
              alert("Genere el arreglo primero")
            }
           
           
        },
        generar(){
          
            for (let index = 0; index < 10; index++) {
              this.arr.push(Math.floor(Math.random()* (100 - 1) + 1));
                      
              
            }

            this.ver=true;
           

            var body = document.getElementById('random')
            var textoCelda = document.createTextNode(this.arr)
            body.appendChild(textoCelda);
            console.log(this.posicion)
                    
        }

            
        }
        
            
        }
      

</script>