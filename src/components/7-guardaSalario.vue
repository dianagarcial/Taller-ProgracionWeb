<template>
<div id="aplicacion">
    <h1>7. Imprimir y guardar 10 salarios</h1>
    <div id="res">
    <input type="number" v-model="salario">
    <button @click="guardar()">Añadir</button>
    <button @click="imprimir()">Imprimir con aumento</button>
    
   </div>
   <h2 id="salarios"></h2>

    </div>
    </template>


<script >


export default {
  
      name:'GuardaSalario',
      data(){
        return{
      
      salario:'',
      arr:[],
      arrem:[],
      ver:false
      
        }

        
      },
      methods:{
        guardar(){
            var numeros = this.salario;
            
                

            var array=this.arr;
            var arregloN=this.arrem;


            if(array.length<=10){
                array.push(numeros);
                console.log(this.arr)
       
                arregloN.push(array[array.length-1]*0.8);
                


            console.log(this.arrem)
            } 
             
           
           
        },
        imprimir(){
            if(this.array===10){
            let res='';
            for (let index = 0; index < this.arrem.length; index++) {
              let element = this.arrem[index];
              res= element +'\n'
              

              
            }
            console.log(this.arrem)
            var body = document.getElementById('salarios')
            var textoCelda = document.createTextNode(res)
            body.appendChild(textoCelda);

            }else{
              alert("Solo se puede visualizar si se han registrado 10 salarios")
            }
            
                
            }

            
        }
        
            
        }
      

</script>