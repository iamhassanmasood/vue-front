<script>
import { ref } from 'vue'
export default {
  setup() {
    const count = ref(0)
    const increment = () => {
      count.value++
    }
    const decrement = () => {
      count.value--
    }

    return {
      count,
      increment,
      decrement
    }
  }
}
</script>

<template>
  <div>
    <h1>Contact</h1>
    <br />
    <button @click="increment" class="btn">+</button>
    <span class="count">{{ count }}</span>
    <button @click="decrement" class="btn">-</button>
    <br />
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
.display {
  margin-top: 10px;
}
</style>
