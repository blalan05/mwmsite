<template>
  <Layout>
    <mega-menu></mega-menu>
    <div class="banner">
      <g-image
        alt="A Mill constructed by MWM as General Contractor"
        src="~/assets/Mill.webp"
        position="bottom right"
      ></g-image>
    </div>
    <div class="highlights__container-wrapper">
      <div class="highlights__container-con">
        <div class="highlights__container-item">
          <g-image src="~/assets/highlight_welding.jpg" alt="Welding Experts" />
          <h3>Welding Experts</h3>
          <p>
            We are really good at what we do, so that’s why we call ourselves
            experts.
          </p>
        </div>
        <div class="highlights__container-item">
          <g-image
            src="~/assets/highlight_custom.jpg"
            alt="Custom Fabrication"
          />
          <h3>Custom Fabrication</h3>
          <p>
            We make custom stuff, and we fabricate it. Thus why we call this
            custom fabrication.
          </p>
        </div>
        <div class="highlights__container-item">
          <g-image src="~/assets/highlight_hiring.jpg" alt="Hiring Experts" />
          <h3>Hiring Experts</h3>
          <p>
            Looking for a job? Well, we are looking for someone better than you,
            so move along.
          </p>
        </div>
        <div class="highlights__container-item">
          <g-image src="~/assets/highlight_promise.jpg" alt="MWM Promise" />
          <h3>MWM Promise</h3>
          <p>
            We will always do the best we can to create a solution to your
            problem.
          </p>
        </div>
      </div>
    </div>
  </Layout>
</template>

<script>
import megaMenu from "../components/megaMenu.vue";
export default {
  metaInfo: {
    title: "Hello, world!",
  },
  components: {
    megaMenu,
  },
};
</script>

<style>
.banner {
  width: 100%;
}
.banner img {
  width: 100%;
}
.highlights__container-wrapper {
  background: #0000aa;
  padding: 2.5em 0;
}
.highlights__container-wrapper div.highlights__container-con {
  width: 88vw;
  margin: 0 auto;
}
.highlights__container-wrapper div.highlights__container-item {
  display: inline-block;
  padding: 0 18px;
  width: 25%;
  text-align: center;
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
</style>
