<script>
export default {
  data() {
    return {
      count: 1
    }
  },
  methods: {
    increment() {
      return this.count++
    },
    decrement() {
      return this.count--
    }
  }
}
</script>
<template>
  <div>
    <h1>Service</h1>
    <br />
    <button @click="increment" class="btn">+</button>
    <span class="count">{{ count }}</span>
    <button @click="decrement" class="btn">-</button>
  </div>
</template>
<style scoped>
.count {
  margin-left: 10px;
  margin-right: 10px;
}
.btn {
  background: hsla(160, 100%, 37%, 1);
  border: none;
  color: white;
  padding: 15px 30px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
}
</style>
