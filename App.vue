<template>
  <div id="app">
    <FormData/>
  </div>
</template>

<script>
import FormData from './components/form-data.vue'

export default {
  name: 'App',
  components: {
    FormData,
  }
}
</script>

<style>
body {
  box-sizing: border-box;
  background: rgb(5, 5, 5);
  display: flex;
}

body::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: linear-gradient(#f00, #f0f);
  clip-path: circle(25% at right 70%);
}

body::after {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: linear-gradient(#670faf, #e91e63);
  clip-path: circle(15% at 5% 10%);
}
</style>
