<template>



   <div id="aplicacion">
    <h1>1. Convertidor de segundos</h1>
    <div id="res">
    <input type="number" v-model="segundos" >
    <h2>{{secondsToString}}</h2>
    </div>
    </div>

    
    

   
   

  
</template>

<script >
export default {
  
      name:'HoraSeg',
      data(){
        return{
      segundos:''
      
        }
      },
      computed: {
        secondsToString() {
            
            var hour = Math.floor(this.segundos / 3600);
            hour = (hour < 10)? '0' + hour : hour;
            var minute = Math.floor((this.segundos / 60) % 60);
            minute = (minute < 10)? '0' + minute : minute;
            var second = this.segundos % 60;
            second = (second < 10)? '0' + second : second;
            
            return  hour + ':' + minute + ':' + second;
            }

}
    
  
  
}
</script>