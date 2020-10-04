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

<style lang="scss" scoped>

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
  font-size: 6.25rem;
}

.absolute-center {
  display: flex; // make use of Flexbox
  align-items: center; // does vertically center the desired content
  justify-content: center; // horizontally centers single line items
  text-align: center; // optional, but helps horizontally center text that breaks into multiple lines
}  
</style>
