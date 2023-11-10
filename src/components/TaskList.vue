<template>
  <ul class="list-group rounded-0">
    <task-item v-for="(task, index) in tasks" :key="index" :task="task" @deleteTask="deleteTask(index)"></task-item>
  </ul>
</template>

<script>
import TaskItem from "./TaskItem.vue";

export default {
  data() {
    return {
      tasks: [
        { text: "Task list and assignments", completed: true },
        { text: "Set due date and assignments", completed: false },
        { text: "Remove duplicate tasks and stories", completed: false },
        { text: "Update the userflow and stories", completed: false },
        { text: "Adjust the components", completed: false },
      ],
    };
  },
  components: {
    TaskItem,
  },
  methods: {
    deleteTask(index) {
      this.tasks.splice(index, 1);
    },
  },
};
</script>