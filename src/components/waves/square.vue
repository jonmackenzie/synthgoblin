

<template>
  <svg
    xmlns="http://www.w3.org/2000/svg"
    viewBox="0 0 56.02 55.95"
    :fill="fillColor"
    :class="{'svg' : !selectedWaveForm }"
  >
    <defs />
    <title>square</title>
    <g id="Layer_11" data-name="Layer 11">
      <path
        class="cls-1"
        d="M4.55,0H51.23C54,.64,55.66,2.21,56,4.74V51.13a5.77,5.77,0,0,1-5,4.82H5.45A6.25,6.25,0,0,1,0,50.89V5.07C.64,2.5,2,.7,4.55,0Z"
      />
    </g>
    <g id="Layer_12" data-name="Layer 12">
      <polyline
        class="cls-2"
        points="10.11 27.3 10.11 23.08 19.27 23.08 19.27 31.8 28.01 31.8 28.01 23.08 36.8 23.08 36.8 31.8 45.97 31.8 45.97 28.02"
      />
    </g>
  </svg>
</template>
<script>
export default {
  name: "square",
  props: {
    selectedWaveForm: {
      type: Boolean,
      default: false
    }
  },
  computed: {
    fillColor() {
      return this.selectedWaveForm ? "#d9d283" : "#70b865";
    }
  }
};
</script>

<style lang="scss" scoped>
.svg {
  &:hover {
    fill: rgb(141, 223, 232);
  }
}
.cls-2 {
  fill: none;
  stroke: #1d1d1b;
  stroke-miterlimit: 10;
}
</style>