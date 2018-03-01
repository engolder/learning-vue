<template>
  <section>
    <ul>
      <transition-group name="list" tag="ul">
        <li v-for="(todoItem, index) in probsdata" :key="todoItem">
          {{ todoItem }}
          <button @click="removeTodo(todoItem, index)">&times;</button>
        </li>
      </transition-group>
    </ul>
  </section>
</template>

<script>
  export default{
    props: ['probsdata'],
    methods: {
      removeTodo(todoItem, index) {
        this.$emit('removeTodo', todoItem, index);
      }
    }
  }
</script>

<style>
  .list-item {
    display: inline-block;
  }
  .list-move {
    transition: transform 1s;
  }
  .list-enter-active, .list-leave-active {
    transition: all 1s;
  }
  .list-enter, .list-leave-to {
    opacity: 0;
    transform: translateY(30px);
  }
</style>
