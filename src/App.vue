<template>
  
<HoraSeg/>
<Llamada/>
<Saludo/>
<TresNumeros/>
<ListaNumeros/>
<ImparMenores/>
<GuardaSalario/>
<PosicionAleatoria/>
<CrearTabla/>
<Matriz></Matriz>
<ObjNotas/>
<ArrNotas/>

<h3>Por Diana Marcela Garcia Lopez - 2190234</h3>
</template>

<script>
// @ is an alias to /src

import Llamada from '@/components/2-llamadas.vue';
import HoraSeg from '@/components/1-horaSegundos.vue';
import Saludo from '@/components/3-saludo.vue';
import TresNumeros from './components/4-tresNumeros.vue';
import ImparMenores from './components/6-imparesMenores.vue';
import ListaNumeros from './components/5-listaNumeros.vue';
import GuardaSalario from './components/7-guardaSalario.vue';
import PosicionAleatoria from './components/8-posicionAleatorio.vue'
import CrearTabla from './components/9-crearTabla.vue';
import Matriz from './components/10-matriz.vue';
import ObjNotas from './components/11-objNotas.vue';
import ArrNotas from './components/12-arrNotas.vue';

export default {
    name:'App',
  components: {
    
    Llamada,
    HoraSeg,
    Saludo,    
    TresNumeros,
    ImparMenores,
    ListaNumeros, 
    GuardaSalario,
    PosicionAleatoria,
    CrearTabla,
    Matriz,
    ObjNotas,
    ArrNotas
    
}
}
</script>

<style>
#aplicacion-der{
  background-color:#EBB2BE;
  padding: 2em;
  margin: 1em;
  border-radius: 1.5em;
  display:flex;
  flex-direction: column;
  width: 45%;
  left: 0;

  
}
#aplicacion-izq{
  background-color:#EBB2BE;
  padding: 2em;
  margin: 1em;
  border-radius: 1.5em;
  display:flex;
  flex-direction: column;
  width: 45%;
  right:  0;


  
}
#aplicacion{
  background-color:#EBB2BE;
  padding: 2em;
  margin: 1em;
  border-radius: 1.5em;
  display:flex;
  flex-direction: column;

  
}
h1{
  font-family: 'Montserrat';
font-style: normal;
font-weight: 500;
font-size: 1em;
line-height: 1.5em;
text-align: left;
text-indent: 5px;
}
h2{
  font-family: 'Montserrat';
font-style: normal;
font-weight: 200;
font-size: 1em;
line-height: 1.5em;
text-align: left;
text-indent: 5px;
}

h3{
  font-family: 'Montserrat';
font-style: normal;
font-weight: 400;
font-size: 0.8em;
line-height: 1.5em;
text-align: right;
text-indent: 5px;
margin:2em
}
#res{
  display: flex;
  flex-direction: row;
  align-items: center;

}

input{
  font-family: 'Montserrat';
font-style: normal;
font-weight: 300;
font-size: 0.8em;
line-height: 1.5em;
text-align: left;
text-indent: 5px;
background-color: antiquewhite;
border-radius: 1em;
outline: none;
border: 0.1em solid #B88C94;
padding: 5px;

}

#tres{
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  width:45%;
}

#nombre{
width: 30%;
}

#hora{
width: 30%;
}

button{
  background-color: #B88C94;
  font-family: 'Montserrat';
font-style: normal;
font-weight: 200;
font-size: 1em;
line-height: 1.5em;
text-align: center;
text-indent: 5px;
color: antiquewhite;
width: 200px;
align-content: center;
border: 0.1em solid #B88C94;
border-radius: 0.2em;
margin-left: 2% ;


}
table 
{   font-family: 'Montserrat';
    font-size: 12px;
    margin: 45px;
    width: 50%;
    text-align: center;    
    border-collapse: collapse; }

th {     font-size: 13px;     font-weight: normal;     padding: 8px;     background: antiquewhite;
    border-top: 4px solid #aabcfe;    border-bottom: 1px solid #fff; color: #B88C94; }

td {    padding: 8px;     background: antiquewhite;     border-bottom: 1px solid #fff;
    color: #9b6871;    border-top: 1px solid transparent; }

tr:hover td { background: rgb(184, 73, 119); color: #B88C94; }


</style>
