<template>
  <div class="highlights__container-wrapper">
    <div class="highlights__container-con">
      <div class="highlights__container-item">
        <div class="highlights__container-img-container">
          <g-image src="~/assets/highlight_welding.jpg" alt="Welding Experts" />
        </div>
        <h3>Welding Experts</h3>
        <div class="highlights__container-item-body">
          <p>
            We are really good at what we do, so that’s why we call ourselves
            experts.
          </p>
        </div>
      </div>
      <div class="highlights__container-item">
        <div class="highlights__container-img-container">
          <g-image
            src="~/assets/highlight_custom.jpg"
            alt="Custom Fabrication"
          />
        </div>
        <h3>Custom Fabrication</h3>
        <div class="highlights__container-item-body">
          <p>
            We make custom stuff, and we fabricate it. Thus why we call this
            custom fabrication.
          </p>
        </div>
      </div>
      <div class="highlights__container-item">
        <div class="highlights__container-img-container">
          <g-image src="~/assets/highlight_hiring.jpg" alt="Hiring Experts" />
        </div>
        <h3>Hiring Experts</h3>
        <div class="highlights__container-item-body">
          <p>
            Looking for a job? Well, we are looking for someone better than you,
            so move along.
          </p>
        </div>
      </div>
      <div class="highlights__container-item">
        <div class="highlights__container-img-container">
          <g-image src="~/assets/highlight_promise.jpg" alt="MWM Promise" />
        </div>
        <h3>MWM Promise</h3>
        <div class="highlights__container-item-body">
          <p>
            We will always do the best we can to create a solution to your
            problem.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "highlights",
};
</script>

<style scoped>
.highlights__container-wrapper {
  background: #000259;
  background-image: url(~@/assets/highlights_bg.jpg);
  padding: 2.5em 0;
  background-blend-mode: screen;
  background-position: top center;
}
.highlights__container-wrapper div.highlights__container-con {
  width: 88%;
  margin: 0 auto;
}
.highlights__container-wrapper div.highlights__container-item {
  display: inline-block;
  padding: 0 18px;
  width: 25%;
  text-align: left;
}
.highlights__container-img-container {
  filter: drop-shadow(3px 3px 4px #1c1a1a);
}
.highlights__container-wrapper div.highlights__container-item img {
  width: 33%;
  min-width: 175px;
  clip-path: polygon(50% 0%, 100% 50%, 50% 100%, 0% 50%);
}
.highlights__container-wrapper div.highlights__container-item h3 {
  color: white;
}
.highlights__container-wrapper div.highlights__container-item p {
  color: white;
  text-align: center;
  max-width: 80%;
}
.highlights__container-item .highlights__container-item-body {
  background: rgba(55, 55, 55, 0.7);
}
.highlights__container-item .highlights__container-item-body p {
  text-align: left;
}
</style>