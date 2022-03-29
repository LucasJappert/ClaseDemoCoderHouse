<template>
    <div class="BotonContador" @click="ClickBotonContador">
        {{count}}
    </div>
</template>

<script>
export default {
    data(){
        return {
            count: 0
        }
    },
    methods: {
        ClickBotonContador(){
            this.count ++;
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