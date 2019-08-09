<template>
  <div id="app">
    {{ message }}
    <Message kek="12dfgdfg345"></Message>
  </div>
</template>

<script>
import Message from './components/Message.vue'

let message = "kek messages";

export default {
    name: 'app',
    data () {
      return {
        message: message
      }
    },
    components: {
      Message
    }
}

</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
