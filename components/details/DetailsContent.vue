<template>
  <div>
    <div id="details" class="is-background-primary is-title">DETAILS</div>
    <div class="details-wrapper">
      <div id="details-left">
        <div class="is-text-bold">Contacts</div>
        <div style="margin-bottom: 15px">
          Victoria, BC, Canada
          <br />brianpham2589@gmail.com
          <br />+1 778 922 6999
          <br />
          <a
            href="https://www.linkedin.com/in/quang-huy-pham-04a82a16b"
            target="_blank"
            rel="noreferrer"
          >LinkedIn</a>
        </div>

        <div class="is-text-bold">Date / Place of birth</div>
        <div>
          08/25/1999
          <br />Hanoi
        </div>
      </div>
      <div id="details-right">
        <div class="is-text-bold">Nationality</div>
        <div style="margin-bottom: 15px">Vietnam</div>

        <div class="is-text-bold">Languages</div>
        <div>
          Vietnamese
          <br />English
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "DetailsContent",
};
</script>

<style scoped>
.details-wrapper {
  display: flex;
}

#details-right {
  margin-left: 400px
}
</style>