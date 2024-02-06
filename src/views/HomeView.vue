<script setup>
import TheWelcome from '../components/TheWelcome.vue'
import ButtonCount from '@/components/ButtonCount.vue'
</script>
<script>
export default {
  data() {
    return {
      input: 0
    }
  }

}
</script>
<template>
  <main>
    <TheWelcome />
    <input type="number" @change="e => input = parseInt(e.target.value) " />
    <ButtonCount :plus="input" />
  </main>
</template>
