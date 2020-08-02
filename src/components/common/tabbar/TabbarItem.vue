<template>
  <div class="tab-bar-item" @click="active">
    <div v-if="!actived"><slot name="img"></slot></div>
    <div v-else ><slot name="activedImg"></slot></div>
    <div :class="{actived: actived}"><slot name="text"></slot></div>
  </div>
</template>

<script>
export default {
  name:"TabbarItem",
  props:{
    path:String
  },
  computed: {
    actived(){
      return this.$route.path === this.path
    }
  },
  methods: {
    active(){
      if(this.$route.path === this.path) return;
      this.$router.push(this.path);
    }
  }
}
</script>

<style scoped>
  img{
    width: 0.2rem;
  }
  .actived{
    color: red;
  }
</style>