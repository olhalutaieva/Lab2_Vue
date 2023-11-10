<template>
    <div class="input-group mb-3">
      <input type="text" v-model="newTask" class="form-control" placeholder="Add a new task" @keyup.enter="addTask" />
      <button @click="addTask" class="btn btn-primary">Add Task</button>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        newTask: "",
      };
    },
    methods: {
      addTask() {
        if (this.newTask.trim() !== "") {
          this.$root.$refs.taskList.tasks.push({ text: this.newTask, completed: false });
          this.newTask = "";
        }
      },
    },
  };
  </script>
  