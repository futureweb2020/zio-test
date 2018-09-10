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
    size: {
      default: 100,
      type: Number
    },
    bgColor: {
      default: 'gray',
      type: String
    },
    centerX: {
      default: 50,
      type: Number
    },
    centerY: {
      default: 50,
      type: Number
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
