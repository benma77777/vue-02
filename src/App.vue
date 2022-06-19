<template>
  <div id="app">
    <ul>
      <li v-for="item in arr" :key="item">
        {{ item }}
      </li>
    </ul>
    <button @click="btn">走一走</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      arr: ["程序员", "帅哥", "美女"],
    };
  },
  methods: {
    btn() {
      // this.arr.push(this.arr[0]);
      // this.arr.shift()

      this.arr.push(this.arr.shift());
    },
  },
};
</script>
<style>
</style>
