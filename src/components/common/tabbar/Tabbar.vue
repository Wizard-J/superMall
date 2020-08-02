<template>
  <div class="tab-bar">
    <slot></slot>
  </div>
</template>

<script>
export default {
  name:"Tabbar"
}
</script>

<style scoped>
  .tab-bar{
  display: flex;
  align-items: center;
  position: fixed;
  height: 0.49rem;
  left: 0;
  right: 0;
  bottom: 0;
  box-shadow: 0 -3px 1px rgba(100, 100, 100, 0.1);
  background-color: #f6f6f6;
}
.tab-bar-item{
  text-align: center;
  flex:1
}
</style>