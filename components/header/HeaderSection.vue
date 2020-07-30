<template>
  <div>
    <nav class="navbar" role="navigation" aria-label="main navigation">
      <div class="navbar-brand">
        <a
          role="button"
          class="navbar-burger burger"
          aria-label="menu"
          aria-expanded="false"
          data-target="navbarBasicExample"
          @click="toggleMenu"
        >
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
        </a>
      </div>

      <div :class="menuActive ? 'navbar-menu is-active' : 'navbar-menu'">
        <div class="navbar-start">
          <a class="navbar-item" href="#detials">Details</a>
          <a class="navbar-item" href="#profile">Profile</a>
          <a class="navbar-item" href="#projects">Projects</a>

          <div class="navbar-item has-dropdown is-hoverable">
            <a class="navbar-link">More</a>

            <div class="navbar-dropdown">
              <a class="navbar-item" href="#education">Education</a>
              <a class="navbar-item" href="#skills">Skills</a>
              <a class="navbar-item" href="#internships">Internships</a>
              <a class="navbar-item" href="#achievements">Achievements</a>
              <a class="navbar-item" href="#future-goals">Future Goals</a>
            </div>
          </div>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: "HeaderSection",
  data() {
    return {
      menuActive: false
    }
  },
  methods: {
    toggleMenu: function () {
      this.menuActive = !this.menuActive;
    },
  }
};
</script>

<style scoped>
.header-section {
  text-align: center;
}

a:link {
  color: black;
  text-decoration: none;
}
a:visited {
  color: black;
  text-decoration: none;
}
a:hover {
  color: black;
  text-decoration: none;
}
a:active {
  color: #bfbfbf;
  text-decoration: none;
}
</style>