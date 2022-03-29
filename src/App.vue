<template>
  <div>
    <b>Soy el componente principal App.vue</b>
    <br>
    <br>
    <MiPrimerComponente/>
  </div>
</template>

<script>
import MiPrimerComponente from "./components/MiPrimerComponente.vue";
import MiSegundoComponente from "./components/MiSegundoComponente.vue";
export default {
  components: {
    MiPrimerComponente,
    MiSegundoComponente
  },
  data() {
    return {
      
    }
  }
}
</script>

<style>
body, html{ 
  margin:0; 
  padding:0; 
  height:100%;
  text-align: center;
  box-sizing: border-box;
  color:white;
  font-family: 'Courier New', Courier, monospace;
  font-size: 24px;
}
#app {
  background-color: #444;
  width: 100%;
  height:100%;
  padding: 20px 10px;
  box-sizing: border-box;
  display:flex;
  justify-content: center;
  text-align: center;
}
</style>
