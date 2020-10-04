<template>
  <div id="background-rect" />
</template>

<script>

export default {
  name: 'App',
  components: {
  }
}
</script>

<style lang="scss" scoped>

#background-rect {
  width: 38%;
  height: 83vh;
  margin: 74px auto;

  background: $color-mauve-dark-purple;
  transform: rotate(9.2deg);

  animation-name: gentle-rotation;
  animation-duration: 10s;
  animation-timing-function: ease;
  animation-iteration-count: infinite;
  animation-direction: alternate;
  animation-fill-mode: backwards;
}

</style>
