<script setup>
import { ref } from 'vue'
import { NButton, datePickerDark, NConfigProvider } from 'naive-ui'

defineProps({
  msg: String
})

const count = ref(0)
</script>

<template>
<nav>
  <ul>
    <li><a href="#">Home</a></li>
      <li><a href="/about">About</a></li>
        <li><a href="/contact">Contact</a></li>
          <li><a href="https://github.com/SteveSimms">Github</a></li>
  </ul>
</nav>
  <h1>{{ msg }}</h1>



  <n-button type="info" @click="count++">count is: {{ count }}</n-button>
   <n-color-picker />

</template>

<style scoped>
a {
  color: #42b983;
}
nav{
  background: #2080f0;
  height: 10vh;
  width: 100vw;
  position: fixed;
  top: 0px;
}
li{
  display: inline-block;
  padding: 2rem;
}
</style>
