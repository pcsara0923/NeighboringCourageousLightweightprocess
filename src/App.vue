<template>
  <div>
    <h1>背景顏色切換工具</h1>
    <div>
      <label for="colorPicker">選擇一個顏色：</label>
      <input type="color" id="colorPicker" v-model="selectedColor" />
    </div>
     <h2 class="selected-color">{{ selectedColor }}</h2>
    <div class="colorBox" :style="{ backgroundColor: selectedColor }">
      <p></p>
     
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      selectedColor: '#ffffff', // 默認白色
    };
  },
};
</script>

<style>
.color-display {
  margin-top: 200px;
  
 
  text-align: center;
} 

.selected-color {
  font-weight: bold;
  color: #333;
}
  .colorBox{
    width:100%;
    height:500px;
  }
</style>
