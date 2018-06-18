<template lang="html">
  <div class="container">
    <h1 class="title">{{ title }}</h1>
    <ul class="projects">
      <Project
        v-for="project in projects"
        :link="project.link"
        :screenshotUrl="project.screenshotUrl"
        :title="project.title"
        :caption="project.caption"
        :tools="project.tools"
      />
    </ul>
  </div>
</template>

<script>
import Project from './Project'

export default {
  name: 'Professional Projects',
  components: {
    Project,
  },
  props: [
    'title',
    'projects',
  ],
}
</script>

<style lang="css" scoped>
.container {
  margin-top: 30px;
  font-family: 'Montserrat', sans-serif;
}
</style>
