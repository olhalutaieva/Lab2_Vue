<template>
    <li class="list-group-item border-0 d-flex align-items-center ps-0">
      <input class="form-check-input me-3" type="checkbox" v-model="task.completed" aria-label="..." />
      <s v-if="task.completed">{{ task.text }}</s>
      <span v-else>{{ task.text }}</span>
    </li>
  </template>
  
  <script>
  export default {
    props: ["task"],
  };
  </script>