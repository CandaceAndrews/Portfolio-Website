<template>
    <div class="project-detail">
      <h2>{{ project && project.projectName }}</h2>
      <p>{{ project && project.description }}</p>
    </div>
  </template>
  
<script>
export default {
  props: {
    project: Object,
  },
};
</script>
  
<style scoped>
.project-detail {
  max-width: 800px;
  margin: 0 auto;
} 
</style>