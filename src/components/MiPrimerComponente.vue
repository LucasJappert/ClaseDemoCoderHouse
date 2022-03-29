<template>
  <div class="MiPrimerComponente">
    <div>
      ¡Hola mundo!
      <br>
      ¡Este es mi primer componente!
      <br>
      <br>
      En el cual instanciaremos varias veces otro nuevo componente "Contador"
      <br>
      <br>
      <div class="ContenedorBotones">
        <Contador />
        <Contador />
        <Contador />
      </div>
    </div>
  </div>
</template>

<script>
import Contador from "./Contador.vue";
export default {
  components: {
    Contador
  },
  data() {
    return {
      
    }
  }
}
</script>

<style scoped>
.MiPrimerComponente{
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