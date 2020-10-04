<template>
  <div id="background" class="absolute-center">
    <div id="background-rect" />
  </div>
  <div id="content" class="absolute-center">
    <div>Coming Soon</div>
  </div>
</template>

<script>

export default {
  name: 'App',
  components: {
  }
}
</script>

<style lang="scss">

#background {
  z-index: 0;
  position: absolute;

  width: 99vw;
  height: 99vh;
}

#background-rect {
  width: 38%;
  height: 83vh;

  background: $color-mauve-dark-purple;
  transform: rotate(9.2deg);

  animation-name: gentle-rotation;
  animation-duration: 10s;
  animation-timing-function: ease;
  animation-iteration-count: infinite;
  animation-direction: alternate;
  animation-fill-mode: backwards;
}

#content {
  position: absolute;
  z-index: 10;

  width: 99vw;
  height: 99vh;

  color: $color-cream;
  font-size: #{"clamp(2.5rem, 0.2119rem + 10.1695vw, 6.25rem)"};
}
</style>
