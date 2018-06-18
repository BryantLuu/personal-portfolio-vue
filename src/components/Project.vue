<template>
  <li class="project">
    <a class="link" :href="link">
      <img class="screenshot" :src="screenshotUrl">
    </a>
    <p class="caption-title">{{ title }}</p>
    <p class="caption">{{ caption }}</p>
  </li>
</template>

<script>
export default {
  name: 'Project',
  props: [
    'link',
    'screenshotUrl',
    'title',
    'caption',
    'tools',
  ],
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.project {
  font-family: 'Montserrat', sans-serif;
}
</style>
