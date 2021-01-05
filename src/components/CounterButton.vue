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
body {
    display: flex;
    align-items: center;
    justify-content: center;
}
.counter-button {
    border-radius: 3px;
    outline: none;
    background: none;
    border: 1px solid #78BC61;
    padding: .5rem 1rem;
    opacity:.8;
    transition: .2s all;
    user-select: none;
    color: #78bc61;
}
.counter-button:hover{
    opacity:1;
    color:white;
    background: #78BC61;
    cursor:pointer;
}
.counter-button:active{
    background: #61974e;
}
</style>