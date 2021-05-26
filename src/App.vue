<template>
  <div id="app">
    <h1>Yassin Eldeep's <span>Very Hard</span> Challenge &#x1F602;&#x1F602;</h1>
    <div>
      <button @click="increment(1)">+1</button>
      <button @click="increment(10)">+10</button>
      <button @click="increment(20)">+20</button>
      <button @click="increment(50)">+50</button>
      <button @click="increment(100)">+100</button>
      <button @click="increment(200)">+200</button>
      <p>{{ num }}</p>
      <button @click="decrement(1)">-1</button>
      <button @click="decrement(10)">-10</button>
      <button @click="decrement(20)">-20</button>
      <button @click="decrement(50)">-50</button>
      <button @click="decrement(100)">-100</button>
      <button @click="decrement(200)">-200</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      num: 0
    }
  },
  methods: {
    increment(amount) {
      this.num+=amount
    },
    decrement(amount) {
      this.num > 0 ? this.num-=amount : this.num
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1 span {
  color: red;
  font-weight: bolder;
  font-size: 50px;
}

p {
  font-size: 35px;
  font-weight: bold;
}

button {
  background-color: #2c3e50;
  color: #FFF;
  text-align: center;
  border: none;
  border-radius: 20px;
  font-size: 20px;
  /*width: 50px;*/
  /*height: 40px;*/
  display: table-cell;
  vertical-align: middle;
  margin-right: 10px;
  padding: 10px 20px
}

button:hover {
  background-color: dimgrey;
}

</style>
