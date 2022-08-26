<template>
<div id="aplicacion">
   <h1>10. Imprimir matriz en una tabla</h1>
   
    
        <table>  
        <tr>
          <td><strong>Codigo</strong></td>
          <td><strong>Valor anterior</strong></td>
          <td><strong>Valor nuevo</strong></td>
        </tr>
        <tr v-for="(quote, index) in items" :key="index + 1">
        

          <td>{{index +1}}</td>
          <td>{{quote.colm1}}</td>
          <td>{{quote.colm2}}</td>
          
        </tr>

        <tr>
          <td></td>
          <td>{{sumcolm1}}</td>
          <td>{{sumcolm2}}</td>
          </tr>

        <tr>
          

        </tr>
        </table>
    
    </div>
    </template>


<script >
export default {
  
      name:'Matriz',
      data(){
        return{
            numero:'',
            items: [
        
            {colm1:5000, colm2:9000},
            {colm1:4000, colm2:3000},
            {colm1:7000, colm2:6000},
            {colm1:9000, colm2:5000}
            ]

    
            
            

       
        }
      },
      computed:{
        sumcolm1(){
          let sum=0
          for (let index = 0; index < this.items.length; index++) {
            var colm= Number(this.items[index].colm1)
            sum=sum+colm;
                       
          }         

          console.log(sum)
          console.log(this.items.length)
          return sum


        },
        sumcolm2(){
          let sum=0
          for (let index = 0; index < this.items.length; index++) {
            var colm= Number(this.items[index].colm2)
            sum=sum+colm;
            
          }
          
          console.log(sum)
          console.log(this.items.length)
          return sum


        }
      }
}
</script>