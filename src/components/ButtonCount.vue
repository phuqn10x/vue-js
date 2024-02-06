<script setup lang="ts">
defineProps({
  plus: {
    type: Number,
    required: true
  },
})
</script>
<script lang="ts">
export default {
  data() {
    return {
      count: 0
    }
  },
  methods :{
    HandleCount()  {
      this.count = this.count + this.plus
    }
  },
  created() {
    console.log(this.plus) // => 2
  }
}



</script>
<template>
  <h1>{{ count }}</h1>
  <button @click="HandleCount"  >Click</button>
</template>

<style scoped>

</style>