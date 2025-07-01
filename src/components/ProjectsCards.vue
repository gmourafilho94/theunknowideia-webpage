<template>
  <div class="project-card">
    <div>
      <span> {{ projects.organizer }} </span>
    </div>
    <span> {{ projects.title }} </span>
    <h4>{{ projects.catchFrase }}</h4>
    <h4>{{ projects.category }}</h4>
    <span> Votes: {{ projects.votes }}</span>
  </div>
</template>

<script>
export default {
  name: 'ProjectsCards',
  props: {
    projects: {
      type: Object,
      required: true,
    },
  },
}
</script>

<style scoped>
.project-card {
  padding: 20px;
  width: 250px;
  cursor: pointer;
  border: 1px solid #39495c;
  margin-bottom: 18px;
}

.project-card:hover {
  transform: scale(1.01);
  box-shadow: 0 3px 12px 0 rgba(0, 0, 0, 0.2);
}
</style>
