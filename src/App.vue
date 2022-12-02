<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <Home />
  <counter />
  <name />
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Home from './components/Home.vue';
import counter from './components/counter.vue'
import name from './components/name.vue'
export default {
  name: 'App',
  components: {
    HelloWorld,
    Home,
    counter,
    name,
  }
}
</script>

