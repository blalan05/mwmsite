<template>
  <Layout>
    <div class="banner">
      <g-image
        alt="A Mill constructed by MWM as General Contractor"
        src="~/assets/Mill.webp"
        position="bottom right"
      ></g-image>
      <p class="mwm_text">Midwest Welding & Manufacturing</p>
      <p class="repair_text">Repairing your past...Fabricating your future.</p>
    </div>
    <services></services>
    <contacts></contacts>
    <highlights></highlights>
    <serviceAreas></serviceAreas>
  </Layout>
</template>

<script>
import contacts from "@/components/contactDetails.vue";
import highlights from "@/components/highlights.vue";
import services from "@/components/services.vue";
import serviceAreas from "@/components/serviceAreas.vue";

export default {
  metaInfo: {
    title: "Hello, world!",
  },
  components: {
    contacts,
    highlights,
    serviceAreas,
    services,
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
.repair_text,
.fabricate_text,
.mwm_text {
  color: #0e133a;
  text-shadow: 1px 1px 2px #1c1a1a;
  font-weight: 600;
  position: absolute;
  z-index: 50;
}
.mwm_text {
  top: 5em;
  left: 2.2em;
  font-size: 36px;
}
.repair_text {
  font-size: 26px;
  top: 10.2em;
  left: 3.7em;
}
.fabricate_text {
  top: 6em;
  left: 5.4em;
}
</style>
