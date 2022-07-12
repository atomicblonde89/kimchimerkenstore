<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div id="app">
    <NavBar />
    <div id="gato">
      gato
    </div>
    <Footer />
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss">
body {
  background: linear-gradient(-45deg, #df1009, #a32c82, #d20056);
  background-size: 400% 400%;
  animation: gradient 15s ease infinite;
  height: 100vh;
}

@keyframes gradient {
  0% {
    background-position: 0% 50%;
  }
  50% {
    background-position: 100% 50%;
  }
  100% {
    background-position: 0% 50%;
  }
}
</style>
