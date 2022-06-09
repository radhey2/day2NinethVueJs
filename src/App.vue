<template>
 <div id="app">
  <h3>What is your favorite kind of taco?</h3>
  <p><input v-model="tacos" /></p>
  <p v-once="tacos">{{ tacos }}</p>
  <span v-pre>This is good if I need to show the mustache view of {{ tacos }}</span>
  <pre>{{ $data }}</pre>
</div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
   data() {
    return {
      tacos: 'I like Al Pastor tacos'
    }
  }
}
</script>
