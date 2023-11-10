<template>
  <div>
    <task-list ref="taskList"></task-list>
    <add-task-form></add-task-form>
    <shared-with-list></shared-with-list>
  </div>
</template>

<script>
import TaskList from "./components/TaskList.vue";
import AddTaskForm from "./components/AddTaskForm.vue";
import SharedWithList from "./components/SharedWithList.vue";

export default {
  components: {
    TaskList,
    AddTaskForm,
    SharedWithList,
  },
};
</script>