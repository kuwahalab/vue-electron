<template>
  <div>
    <div
      v-for="(value, index) in buttons"
      :key="index"
    >
      <button
        v-for="item in value"
        :key="item"
      >
        {{ item }}
      </button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      buttons: [
        ["AC", "+/-", "%", "/"],
        [7, 8, 9, "*"],
        [4, 5, 6, "-"],
        [1, 2, 3, "+"],
        [0, ".", "="]
      ]
    }
  }
}
</script>