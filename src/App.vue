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
    <Projects
      title="Professional Profile"
      :projects="professionalProjects"
    />
    <Projects
      title="Side Projects"
      :projects="professionalProjects"
    />
  </div>
</template>

<script>
import Projects from './components/Projects';

export default {
  name: 'App',
  components: {
    Projects,
  },
  data() {
    return {
      professionalProjects: [
        {
          link: "www.reddit.com",
          screenshotUrl: "url",
          title: "Carta",
          caption: "Full-stack software engineer",
          tools: "Python | Django",
        },
        {
          link: "www.reddit.com",
          screenshotUrl: "url",
          title: "Carta",
          caption: "Full-stack software engineer",
          tools: "Python | Django",
        },
        {
          link: "www.reddit.com",
          screenshotUrl: "url",
          title: "Carta",
          caption: "Full-stack software engineer",
          tools: "Python | Django",
        },
      ],
    }
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
    overflow: hidden;
  }
  .bio {
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
</style>
