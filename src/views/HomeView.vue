<template>
  <div class="projects">
    <h1>Upcoming Projects</h1>
    <ProjectsCards
      v-for="project in projects"
      :key="project.id"
      :projects="project"
    />
  </div>
</template>

<script>
// @ is an alias to /src
import ProjectsCards from '@/components/ProjectsCards.vue'
export default {
  name: 'home-view',
  components: {
    ProjectsCards,
  },
  data() {
    return {
      projects: [
        {
          id: 5928101,
          category: 'tech',
          catchFrase: 'lorem projlasjdoicae',
          title: 'Cat Adoption Day',
          description: 'Find your new feline friend at this event.',
          votes: 10,
          organizer: 'Kat Laydee',
        },
        {
          id: 5928102,
          category: 'tech',
          catchFrase: 'lorem projlasjdoicae',
          title: 'Cat Adoption Day',
          description: 'Find your new feline friend at this event.',
          votes: 10,
          organizer: 'Kat Laydee',
        },
        {
          id: 5928103,
          category: 'tech',
          catchFrase: 'lorem projlasjdoicae',
          title: 'Cat Adoption Day',
          description: 'Find your new feline friend at this event.',
          votes: 10,
          organizer: 'Kat Laydee',
        },
      ],
    }
  },
}
</script>

<style scoped>
.projects {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
