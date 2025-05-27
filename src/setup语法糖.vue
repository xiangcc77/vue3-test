<!-- <script>
export default {
  setup () {
    const message = 'hello world'

    const logMessage = () => {
      console.log(message)
    }

    return {
      message,
      logMessage
    }
  }
}
</script> -->


<script setup>
  const message = 'hello world'

  const logMessage = () => {
      console.log(message)
    }
</script>

<template>
  <div>{{ message }}</div>
  <button @click="logMessage">按钮</button>
</template>


<style scoped>
</style>