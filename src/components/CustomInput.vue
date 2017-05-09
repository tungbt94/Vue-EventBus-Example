<template>
  <div class="input-vue">
    <span>Your name:</span>
    <input id="input-message" type="text" @input="inputChange">
  </div>
</template>

<script>
import { EventBus } from '../event-bus.js'

export default {
  methods: {
    inputChange() {
      let message = document.getElementById('input-message').value;
      EventBus.$emit('inputChanged', message);
    }
  }
}
</script>
