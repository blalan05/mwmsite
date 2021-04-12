<template>
  <Layout>
    <div class="banner">
      <g-image
        alt="A Mill constructed by MWM as General Contractor"
        src="~/assets/Mill.webp"
        position="bottom right"
      ></g-image>
    </div>
    <services></services>
    <contacts></contacts>
    <highlights></highlights>
  </Layout>
</template>

<script>
import contacts from "@/components/contactDetails.vue";
import highlights from "@/components/highlights.vue";
import services from "@/components/services.vue";

export default {
  metaInfo: {
    title: "Hello, world!",
  },
  components: {
    contacts,
    highlights,
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
</style>
