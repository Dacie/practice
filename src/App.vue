<template>
  <div>
    <canvas id="canvas" width="300" height="300"></canvas>
    <button id="button" @click="click">点击移动</button>
  </div>
</template>

<script>

export default {
  mounted(){
    var c = document.getElementById("canvas").getContext("2d");
    console.log(c)
    c.fillStyle = 'skyblue';
    c.fillRect(0,0,300,300);
  },
  methods: {
    click(){

    }
  }
}
</script>

<style>
#canvas {
  border: none;
  position: relative;
  left: 600px;
  top: 200px;
}
#button{
  border: none;
  width: 100px;
  height: 50px;
  font-size: 18px;
  position: relative;
  left: 400px;
  top: 280px;
}
</style>
