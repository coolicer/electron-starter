<template>
  <div id="app" class="main">
    <div class="main-left">
      <div class="main-left-video">video</div>
      <div class="main-left-meta">
        <div class="meta-up">up</div>
        <div class="meta-down">down</div>
      </div>
    </div>
    <div class="main-aside">aside</div>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld
  },
}
</script>

<style lang="less">
html, body {
  width: 100%;
  height: 100%;
  overflow: hidden;
}
.main {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  display: flex;
  height: 100%;
  min-width: 1000px;
  &-left {
    flex-grow: 1;
    background-color: #f0c;
    &-video {
      height: 60vh;
      background-color: #fc0;
    }
    &-meta {
      display: flex;
      flex-direction: column;
      height: 40vh;
      .meta-up {
        flex: 1;
        background-color: #fcc;
      }
      .meta-down {
        flex: 1;
        background-color: #dfd;
      }
    }
  }
  &-aside {
    flex-basis: 400px;
    width: 400px;
    background-color: #fff;
  }
}
</style>
