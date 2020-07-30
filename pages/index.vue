<template>
  <div class="container">
    <HeadingContent />
    <DetailsContent />
    <ProfileContent />
    <EducationContent />
    <SkillContent />
    <InternshipsContent />
    <AchievementsContent />
    <GoalsContent />
    <div class="divider" />
    <ProjectContent />
  </div>
</template>

<script>
import HeadingContent from "../components/heading/HeadingContent.vue";
import DetailsContent from "../components/details/DetailsContent.vue";
import ProfileContent from "../components/profile/ProfileContent.vue";
import EducationContent from "../components/education/EducationContent.vue";
import SkillContent from "../components/skills/SkillContent.vue";
import InternshipsContent from "../components/internships/InternshipsContent.vue";
import AchievementsContent from "../components/achievements/AchievementsContent.vue";
import GoalsContent from "../components/goals/GoalsContent.vue";
import ProjectContent from "../components/projects/ProjectsContent.vue";

export default {
  head() {
    return {
      title: "Brian Pham's e-portfolio",
      meta: [
        {
          hid: "portfolio",
          name: "portfolio",
          content: "Brian Pham e-portfolio",
        },
      ],
    };
  },
  components: {
    HeadingContent,
    DetailsContent,
    ProfileContent,
    EducationContent,
    SkillContent,
    InternshipsContent,
    AchievementsContent,
    GoalsContent,
    ProjectContent
  },
};
</script>

<style>
.container {
  margin: 20px 100px 20px 100px;
  font-family: "Lucida Console", Courier, monospace;
}

a:link {
  color: black;
  text-decoration: underline;
}
a:visited {
  color: black;
  text-decoration: underline;
}
a:hover {
  color: black;
  text-decoration: underline;
}
a:active {
  color: #bfbfbf;
  text-decoration: underline;
}
</style>
