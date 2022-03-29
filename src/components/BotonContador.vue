<template>
  <div @click="AumentarContador()" class="BotonContador">
      Count: {{count}}
  </div>
</template>

<script>
  
export default {
  components: {
  },
  props: ['initialCount'],
  mounted(){
      this.SetCount(this.initialCount);
  },
  data() {
    return {
      count: 0//this.initialCount ?? 0
    }
  },
  methods: {
      AumentarContador(){
          this.count ++;
      },
      SetCount(count){
        if (count)
            this.count = count;
        else
            this.count = 0;
      }
  }
}
</script>

<style scoped>
.BotonContador{
    width:200px; height:50px;
    border-radius: 10px;
    background-color: #CCC;
    color: #000;
    border:1px solid #000;
    box-sizing: border-box;
    display: flex;
    justify-content: center;
    align-items: center;
    margin:10px;
    padding:0 10px;
    cursor: pointer;
    user-select: none;
    font-weight: bold;
}
</style>