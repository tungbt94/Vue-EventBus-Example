<template>
  <div id="app">
    <custom-input></custom-input>
    <welcome></welcome>
  </div>
</template>

<script>
import CustomInput from './components/CustomInput.vue'
import Welcome from './components/Welcome.vue'
export default {
  name: 'app',
  components: {
    'custom-input': CustomInput,
    'welcome': Welcome
  }
}
</script>
