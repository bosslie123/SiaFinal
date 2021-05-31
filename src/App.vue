<template>
  <div id="app">
    <task v-bind:tasks="tasks"></task>
  </div>
</template>

<script>
import Task from "./components/Task";

export default {
  name: "App",
  components: {
    Task,
  },
  data() {
    return {
      tasks: [
        {
          id: 1,
          title: "Electric Fan",
          completed: true,
        },
        {
          id: 2,
          title: "Rice Cooker",
          completed: true,
        },
        {
          id: 3,
          title: "Pineapple Juice",
          completed: false,
        },
        {
          id: 4,
          title: "Lumpia Wrapper",
          completed: false,
        },
        {
          id: 5,
          title: "Vegetables",
          completed: false,
        },
      ],
    };
  },
};
</script>