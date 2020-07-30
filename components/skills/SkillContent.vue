<template>
  <div>
    <div id="profile" class="is-background-primary is-title">SKILLS</div>
    <div class="skills-wrapper">
      <div id="skills-left">
        <div>Front-end Development</div>
        <ProgressBar :stepsCompleted="3" :totalSteps="5" />
        <div>JavaScript</div>
        <ProgressBar :stepsCompleted="3" :totalSteps="5" />
        <div>React.JS / Next.JS</div>
        <ProgressBar :stepsCompleted="3" :totalSteps="5" />
      </div>
      <div id="skills-right">
        <div>Vue.JS / Nuxt.JS</div>
        <ProgressBar :stepsCompleted="2" :totalSteps="5" />
        <div>Python</div>
        <ProgressBar :stepsCompleted="3" :totalSteps="5" />
        <div>Java</div>
        <ProgressBar :stepsCompleted="3" :totalSteps="5" />
      </div>
    </div>
  </div>
</template>

<script>
import ProgressBar from "../static/ProgressBar.vue";

export default {
  components: {
    ProgressBar,
  },
};
</script>

<style scoped>
.skills-wrapper {
  display: flex;
}

#skills-right {
  margin-left: 400px;
}
</style>