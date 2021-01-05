<template>
  <button @click="add" class="counter-button">I've been clicked {{ count }} times.</button>
</template>

<script>
export default {
  data() {
    return {
      count: 0,
    };
  },
  methods: {
    add() {
      this.count += 1;
    },
  },
};
</script>

<style>
.counter-button {
    border-radius: 5px;
    outline: none;
    background-color: none;
    border: 2px solid #F4D35E;
}
</style>