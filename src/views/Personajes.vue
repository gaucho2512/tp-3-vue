<template>
<div> 

   <!-- Componente NABVAR -->
   <Navbar />
  
  <!-- Seccion Central TABLA -->
  <div class="section-personajes">
         <div>
          <img class="imagen-trans" src="../assets/fondo-personajes2.jpg" alt="foto fondo">
        </div>
  </div>

  <!-- Componente Tabla -->
  <Tabla />
  
  <!-- Componente FOOTER  -->
  <Footer />

  </div>
</template>

<script>

import Navbar from "../components/Navbar"
import Footer from "../components/Footer"
import Tabla from "../components/Tabla"

export default {
  components: {
    Navbar,
    Tabla,
    Footer,
  },
}
  
</script>

<style>
       
.section-personajes {
    width: 100%;
    max-height: 50%;
    display: flex;
}

.imagen-trans {
    display: flex;
    /* position: absolute; */
    top: 100px;
    left: 0;
}
    
.titulo-personajes{
    text-align: center;
    font-size: 20px;
    text-decoration: underline;
    padding: 25px;
}

.td-Head{
    background-color: #f4f4f4;
    border: solid 1px black;
    padding: 14px;
    font-size: 18px;
    font-weight: bold;   
}

.td-Elementos{
   border: 1px solid black;
   padding: 6px;
}

.btn-accion{
    margin-top: 5px;
    margin-right: 5px;
    display: inline-block;
    width: 75px;
    border-radius: 5px;
    padding: 1px;
    margin-bottom: 5px;
}
 
/* progress bar */
.btn-spinner {
    display: flex;
    margin-bottom: px;
    margin-left: 573px;
}

.hidden{
    visibility: hidden;
}

.visible{
    visibility: visible;
}

.none{
   display: none;
}

.block{
    display: block;
}

/* Toggle Bar */
.switch {
    position: relative;
    display: inline-block;
    width: 60px;
    height: 34px;
    margin-top: 28px;
    margin-left: 127px;
}
  
.switch input { 
  opacity: 0;
  width: 0;
  height: 0;
}
  
.slider {
  position: absolute;
  cursor: pointer;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: #ccc;
  -webkit-transition: .4s;
  transition: .4s;
}

.slider:before {
  position: absolute;
  content: "";
  height: 26px;
  width: 26px;
  left: 4px;
  bottom: 4px;
  background-color: white;
  -webkit-transition: .4s;
  transition: .4s;
}

input:checked + .slider {
  background-color: #2196F3;
}

input:focus + .slider {
  box-shadow: 0 0 1px #2196F3;
}

input:checked + .slider:before {
  -webkit-transform: translateX(26px);
  -ms-transform: translateX(26px);
  transform: translateX(26px);
}

/* Rounded sliders */
.slider.round {
  border-radius: 34px;
}

.slider.round:before {
  border-radius: 50%;
}

/*  @ MEDIA  */

</style>