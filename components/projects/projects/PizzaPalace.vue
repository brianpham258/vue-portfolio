<template>
  <div>
    <div class="card">
      <div class="card-image">
        <figure class="image">
          <img src="../../../static/img/PizzaPalaceHome.png" alt="Pizza Palace" />
        </figure>
      </div>
      <div class="card-content">
        <div class="media">
          <div class="media-content">
            <p class="title is-4">Pizza Palace</p>
          </div>
        </div>

        <div class="content">A small project to get to know HTML, CSS, Bootstrap, and PHP</div>
      </div>
      <footer class="card-footer">
        <button class="card-footer-item button" @click="showPizzaModal">See more</button>
      </footer>
    </div>

    <!-- Modal -->
    <div :class="pizzaModalActive ? 'modal is-active' : 'modal'">
      <div class="modal-background"></div>
      <div class="modal-card">
        <header class="modal-card-head">
          <p class="modal-card-title">Pizza Palace</p>
          <button class="delete" aria-label="close" @click="hidePizzaModal"></button>
        </header>
        <section class="modal-card-body">
          <!-- Content ... -->
          <p>
            This is a small project I made after finished a
            Web Development course at Camosun. It just a simple website
            that used HTML, CSS, Bootstrap, PHP, and Google Map plugin to
            represent a random pizza website that doesn't exist. The
            website's back-end is running on PHP and it could handle
            the pizza ordering process but you will never receive your
            pizza.
          </p>
          <br />
          <a
            href="http://deepblue.cs.camosun.bc.ca/~ics057/ics111/lab04/PizzaPalace/index.html"
            target="_blank"
            rel="noreferrer"
          >Checkout the website here.</a>
          <img
            class="has-margin-bottom"
            alt="Pizza Palace Home"
            src="../../../static/img/PizzaPalaceHome.png"
          />
          <div class="divider" />
          <img
            class="has-margin-bottom"
            alt="Pizza Palace Menu"
            src="../../../static/img/PizzaPalaceMenu.png"
          />
          <div class="divider" />
          <img
            class="has-margin-bottom"
            alt="Pizza Palace Order"
            src="../../../static/img/PizzaPalaceOrder.png"
          />
        </section>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "PizzaPalace",
  data() {
    return {
      pizzaModalActive: false,
    };
  },
  methods: {
    showPizzaModal: function () {
      this.pizzaModalActive = true;
    },
    hidePizzaModal: function () {
      this.pizzaModalActive = false;
    },
  },
};
</script>

<style scoped>
</style>