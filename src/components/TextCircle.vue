<template>
  <svg :height="size" :width="size" :style="{ position: 'absolute', left: centerX, top: centerY, transform: 'translate(-50%, -50%)' }">
    <circle cx="50%" cy="50%" r="50%" :fill="bgColor" />
    <text x="50%" y="50%" alignment-baseline="middle" text-anchor="middle">{{ text }}</text>
  </svg>
</template>

<script>
export default {
  name: 'TextCircle',
  props: {
    text: String,
    size: {
      default: 100,
      type: Number
    },
    bgColor: {
      default: 'gray',
      type: String
    },
    centerX: {
      default: 0,
      type: Number
    },
    centerY: {
      default: 0,
      type: Number
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
