<template>
  <div id="app">
    <div class="cover">
      <div class="bio">
        <div class="container">
          <h1 class="title">Bryant Luu</h1>
          <p class="bio-text">
            I am a business-minded software engineer
            who strives to understand the underlying business problem engineers
            should be solving. I deliver high-quality products on-time under
            rigid business constraints.
          </p>
          <p class="bio-text">
            My interests lie at the intersection of software development,
            user experience, and design. I am always looking for an
            environment and culture where talent is cultivated, knowledge is shared,
            and passion is requisite.
          </p>
        </div>
      </div>
    </div>
    <ProfessionalProjects />
    <SideProjects />
  </div>
</template>

<script>
import ProfessionalProjects from './components/ProfessionalProjects';
import SideProjects from './components/SideProjects';

export default {
  name: 'App',
  components: {
    ProfessionalProjects,
    SideProjects,
  },
};
</script>

<style>
  #app {
    font-family: 'Libre Baskerville', serif;
    color: #666;
    background-color: white;
  }
  .bio-text {
    line-height: 1.6em;
  }
  .cover {
    position: relative;
    height: 360px;
    overflow: hidden;
  }
  .bio {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    padding-top: 30px;
    border-bottom: 2px solid #aaa;
    padding: 30px;
    display: block;
  }
  .caption-title {
    color: #666;
  }
  .caption {
    color:#aaa;
  }
  .projects {
    display: flex;
    justify-content: space-between;
    padding-left: 0px;
  }
  .project {
    display: inline-block;
  }
  .container {
    width: 1000px;
  }
  .video {
    min-width: 100%;
    object-fit: contain;
    max-height: 500px;
  }
</style>
