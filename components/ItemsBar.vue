<template>
    <div class="parent-container">
  <div class="child-container">
    <div class="left">
      <p>items</p>
      <p>Hide Filter</p>
    </div>
    <div class="right">
      <div class="dropdown">RECOMMENDED
        <img src="/assets/arrow-left.png" alt="">
      </div>
    </div>
  </div>
  <LeftItembar/>
</div>
  
  
</template>
<script>
import LeftItembar from './LeftItembar.vue';
export default {
    components:{
        LeftItembar
    }
}
</script>
<style scoped>
.child-container {
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 100%;
  max-width: 1248px;
  margin: 0 auto;
}
.parent-container{
    width: 100%;
  max-width: 1248px;
}
.left {
  display: flex;
  width: 20%;
  padding: 10px;
  align-items: center;
  gap: 20px;
  justify-content: space-between;
}
.left p:nth-child(1) {
  font-family: 'Norm', sans-serif;
  font-size: 18px;
  font-weight: 700;
  line-height: 40px;
  text-align: left;
  text-transform: uppercase;
}
.left p:nth-child(2) {
  color: #888792;
}
.right {
  font-family: 'Norm'sans-serif;
  font-size: 15px;
  font-weight: 700;
  line-height: 40px;
  text-align: left;
}
.dropdown{
    display: flex;
    align-items: center;
}
</style>
