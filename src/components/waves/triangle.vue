

<template>
  <svg
    xmlns="http://www.w3.org/2000/svg"
    viewBox="0 0 56.02 55.95"
    :fill="fillColor"
    :class="{'svg' : !selectedWaveForm }"
  >
    <defs />
    <title>triangle</title>
    <g id="knapp2">
      <path
        class="cls-1"
        d="M4.55,50.84H51.23c2.81.64,4.43,2.21,4.79,4.74V102a5.77,5.77,0,0,1-5,4.82H5.45A6.25,6.25,0,0,1,0,101.73V55.91C.64,53.34,2,51.54,4.55,50.84Z"
        transform="translate(0 -50.84)"
      />
    </g>
    <g id="Layer_9" data-name="Layer 9">
      <polyline
        class="cls-2"
        points="10.07 27.98 14.43 23.9 23.58 32.21 32.51 23.9 41.66 32.21 45.91 28.05"
      />
    </g>
  </svg>
</template>
<script>
export default {
  name: "triangle",
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