<template>
  <div id="app">
    <!-- 간단한 앱이지만 연습을 위해 4개의 컴포넌트로 나눕니다 -->

    <!-- 
      컴포넌트 파트를 참고하세요
     -->
    <TodoHeaderVue></TodoHeaderVue>
    <TodoInputVue @addTodo="addTodo"></TodoInputVue>
    <TodoListVue :probsdata="todoItems" @removeTodo="removeTodo"></TodoListVue>
    <TodoFooterVue @removeAll="clearAll"></TodoFooterVue>
  </div>
</template>

<script>
// ES6의 문법입니다
// .vue파일을 가져옵니다
import TodoHeaderVue from './components/TodoHeader.vue';
import TodoInputVue from './components/TodoInput.vue';
import TodoFooterVue from './components/TodoFooter.vue';
import TodoListVue from './components/TodoList.vue';

  export default{
    // 단일 파일 컴포넌트는 데이터를 함수로서 표현합니다
    data() {
      return {
        todoItems: []
      }
    },
    created() {
      // 브라우저의 로컬 스토리지을 사용해서 todo list 데이터를 관리합니다
      // 뷰 객체가 생성되는 시점에 로컬 스토리지에서 데이터를 가져옵니다
      for(var i = 0; i < localStorage.length; i++) {
        this.todoItems.push(localStorage.key(i));
      }
    },
    methods: {
      addTodo(todoItem) {
        localStorage.setItem(todoItem, todoItem);
        this.todoItems.push(todoItem);
      },
      clearAll() {
        localStorage.clear();
        this.todoItems = [];
      },
      removeTodo(todoItem, index) {
        localStorage.removeItem(todoItem);
        this.todoItems.splice(index, 1);
      }
    },
    components: {
      'TodoHeaderVue': TodoHeaderVue,
      'TodoInputVue': TodoInputVue,
      'TodoListVue': TodoListVue,
      'TodoFooterVue': TodoFooterVue,
    }
  }
</script>

<style>
  body {
    text-align: center;
  }
  button {
    display: inline-block;
    height: 30px;
    min-width: 30px;
  }
</style>
