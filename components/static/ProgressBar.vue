<template>
  <div class="progress-bar-wrapper">
    <div v-for="step in stepsCompleted" :key="step" class="is-completed" />
    <div v-for="step in totalSteps - stepsCompleted" :key="step" class="is-not-complete" />
  </div>
</template>

<script>
export default {
  name: "ProgressBar",
  props: {
    stepsCompleted: Number,
    totalSteps: Number,
  }
};
</script>

<style scoped>
.progress-bar-wrapper {
  display: flex;
  height: 7px;
  margin-top: 10px;
}

.is-completed {
  border-radius: 25px;
  width: 40px;
  margin-right: 5px;
  background-color: #000000;
}

.is-not-complete {
  border-radius: 25px;
  width: 40px;
  margin-right: 5px;
  background-color: #bfbfbf;
}
</style>