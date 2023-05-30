<script>
export default {
  data() {
    return {
      tasks: [
        { id: 1, title: 'Tâche 1', completed: false },
        { id: 2, title: 'Tâche 2', completed: true },
        { id: 3, title: 'Tâche 3', completed: false }
      ]
    }
  }
}

</script>
<template>
    <div class="task-wrapper">
        <div class="task" v-for="task in tasks" :key="task.id">
            <input type="checkbox" class="task-item" :id="task.id">
            <label>{{ task.title }}</label>
        </div>
    </div>
</template>