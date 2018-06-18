<template lang="html">
  <div class="container">
    <h1 class="title">Side Projects</h1>
    <ul class="projects">
      <Project
        link="www.reddit.com"
        screenshotUrl="url"
        title="Carta"
        caption="Full-stack software engineer"
        tools="Python | Django"
      />
      <Project
        link="www.reddit.com"
        screenshotUrl="url"
        title="Carta"
        caption="Full-stack software engineer"
        tools="Python | Django"
      />
      <Project
        link="www.reddit.com"
        screenshotUrl="url"
        title="Carta"
        caption="Full-stack software engineer"
        tools="Python | Django"
      />
    </ul>
  </div>
</template>

<script>
import Project from './Project'

export default {
  name: 'SideProjects',
  components: {
    Project,
  },
}
</script>

<style lang="css">
.container {
  font-family: 'Montserrat', sans-serif;
}
</style>
