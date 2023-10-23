<script>
export default {
  data() {
    return {
      obj: {
        nested: { count: 0 },
        arr: ['foo', 'bar']
      }
    }
  },
  methods: {
    increment() {
      return this.obj.nested.count++
    },
    decrement() {
      return this.obj.nested.count--
    },
    mutateDeeply() {
      this.obj.nested.count++
      this.obj.arr.push('baz')
    }
  }
}
</script>
<template>
  <div>
    <h1>Service</h1>
    <br />
    <button @click="increment" class="btn">+</button>
    <span class="count">{{ obj.nested.count }}</span>
    <button @click="decrement" class="btn">-</button>
    <br />
    <button @click="mutateDeeply" class="btn display">Mute Display</button>
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
