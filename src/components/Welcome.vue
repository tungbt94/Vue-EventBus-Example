<template>
  <p>Hello {{message}}!</p>
</template>

<script>
import { EventBus } from '../event-bus.js'

export default {
  data() {
    return {
      message: ''
    }
  },
  mounted() {
    console.log("mounted");
    EventBus.$on("inputChanged", (messageUpdated) => {
      this.message = messageUpdated;
    })
  }
}
</script>
