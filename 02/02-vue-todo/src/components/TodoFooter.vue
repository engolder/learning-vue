<template>
  <button @click="clearTodo">Clear All</button>
</template>

<script>
  export default{
    methods: {
      clearTodo() {
        this.$emit('removeAll');
      }
    }
  }
</script>

<style>
</style>
