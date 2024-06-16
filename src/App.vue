<script>
// Импортируем компонент HelloWorld.vue
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld // Регистрируем компонент в опциях компонента
  }
}
</script>

<template class="grid">
  <h1 class="text-3xl text-center font-bold underline">Hello world!</h1>
  <div class="text-center width-300 ">
    <HelloWorld />
    <p>Lorem, ipsum.</p>
  </div>
  <h2 class="text-right">New News</h2>
</template>

<style>
body {
  background-color: rgb(224, 8, 66);
}
</style>
