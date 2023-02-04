<script>
export default {
  data() {
    return {
      count: 0,
    }
  },
  methods: {
    increment() {
      this.count++;
    },
    decrement() {
      this.count--;
    }
  }
}
</script>

<template>
  <div id="counter">
    <button @click="increment">+1</button>
    <h1>{{ count }}</h1>
    <button @click="decrement">-1</button>
  </div>
</template>

<style scoped>
  #counter {
    display: flex;
    gap: 2rem;
  }

  #counter button {
    border-radius: 1rem;
    border: 1px solid black;
    cursor: pointer;
  }
</style>
