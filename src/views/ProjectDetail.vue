
<template>
  <div class="project-detail">
    <h1>{{ project.projectName }}</h1>
    <img class="detail-image" :src="project.thumbnailSource" :alt="project.projectName">
    <p>{{ project.description }}</p>
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
padding: 50px;
}

.detail-image {
  max-width: 100%;
  height: auto;
  margin-bottom: 15px;
}
</style>