<template>
  <div>
    <svg :height="size" :width="size">
      <circle cx="50%" cy="50%" r="50%" :fill="bgColor" />
      <text :x="centerX" :y="centerY" alignment-baseline="middle" text-anchor="middle">{{ text }}</text>
    </svg>
  </div>
</template>

<script>
export default {
  name: 'TextCircle',
  props: {
    text: String,
    size: Number,
    bgColor: String,
    centerX: Number,
    centerY: Number
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
