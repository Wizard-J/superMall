<template>
  <div id="app">
    <h2>app</h2>
    <router-link to="/home">首页</router-link>
    <router-link to="/about">关于</router-link>
    <keep-alive>
      <router-view></router-view>
    </keep-alive>
  </div>
</template>

<style>
@import "assets/css/normalize.css";
</style>
