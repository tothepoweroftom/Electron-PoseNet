<template>
  <div id="wrapper">
    <main>
      <h1>PoseNet Example</h1>
      <canvas id="canvas" width="640" height="480"></canvas> 
      <video id="video" width="640" height="480" autoplay style="display: none"></video>
    </main>
  </div>
</template>

<script>
  import run from './sketch.js'
  export default {
    name: 'landing-page',
    components: {},
    methods: {},
    mounted () {
      run()
    }
  }
</script>

<style>
  @import url('https://fonts.googleapis.com/css?family=Source+Sans+Pro');

  * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }

  body { font-family: 'Source Sans Pro', sans-serif; }

  #wrapper {
    background:
      radial-gradient(
        ellipse at top left,
        rgba(255, 255, 255, 1) 40%,
        rgba(229, 229, 229, .9) 100%
      );
    height: 100vh;
    padding: 60px 80px;
    width: 100vw;
  }

  #logo {
    height: auto;
    margin-bottom: 20px;
    width: 420px;
  }

  main {
    display: flex;
    justify-content: space-between;
  }

  main > div { flex-basis: 50%; }
</style>
