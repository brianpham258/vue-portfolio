<template>
  <div>
    <div class="card">
      <div class="card-image">
        <figure class="image">
          <img src="../../../static/img/TukTukHeavenHome.png" alt="Capstone" />
        </figure>
      </div>
      <div class="card-content">
        <div class="media">
          <div class="media-content">
            <p class="title is-4">Tuk Tuk Heaven</p>
          </div>
        </div>

        <div
          class="content"
        >A small project to practice making single page website</div>
      </div>
      <footer class="card-footer">
        <button class="card-footer-item button" @click="showTukTukModal">See more</button>
      </footer>
    </div>

    <!-- Modal -->
    <div :class="tuktukModalActive ? 'modal is-active' : 'modal'">
      <div class="modal-background"></div>
      <div class="modal-card">
        <header class="modal-card-head">
          <p class="modal-card-title">Tuk Tuk Heaven</p>
          <button class="delete" aria-label="close" @click="hideTukTukModal"></button>
        </header>
        <section class="modal-card-body">
          <!-- Content ... -->
          <p>
            This is also a small project I made after finished a
            Web Development course. This is a singple page website
            that was built on HTML, CSS, and Bootstrap. It represents an
            imagination store that sells tuk tuk. It doesn't have any
            back-end, it just simply displaying the products, price,
            and some informations
          </p>
          <br />
          <a
            href="http://deepblue.cs.camosun.bc.ca/~ics057/ics111/lab05/index.html"
            target="_blank"
            rel="noreferrer"
          >Checkout the website here.</a>
          <img
            class="has-margin-bottom"
            alt="Tuk Tuk Heaven Home"
            src="../../../static/img/TukTukHeavenHome.png"
          />
          <div class="divider" />
          <img
            class="has-margin-bottom"
            alt="Tuk Tuk Heaven Product"
            src="../../../static/img/TukTukHeavenProducts.png"
          />
        </section>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TukTukHeaven",
  data() {
    return {
      tuktukModalActive: false,
    };
  },
  methods: {
    showTukTukModal: function () {
      this.tuktukModalActive = true;
    },
    hideTukTukModal: function () {
      this.tuktukModalActive = false;
    },
  },
};
</script>

<style scoped>
</style>