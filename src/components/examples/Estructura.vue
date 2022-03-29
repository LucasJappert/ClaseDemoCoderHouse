<template>
  <div class="demo">
    Este es mi segundo componente, el cual contiene varias instancias de otro componente "BotonContador":
    <br>
    <div class="ContenedorBotones">
        <BotonContador initialCount=26 />
        <BotonContador initialCount=0 />
        <BotonContador />
    </div>
  </div>
</template>

<script>
import BotonContador from './BotonContador.vue';
  
export default {
  components: {
    BotonContador,
  },
  data() {
    return {
      
    }
  }
}
</script>

<style scoped>
.demo{
  background-color: #666;
  text-align: center;
  padding: 5px;
  width:100%;
  box-sizing: border-box;
}
.ContenedorBotones{
    display:flex;
    justify-content: center;
    align-items: center;
}
</style>