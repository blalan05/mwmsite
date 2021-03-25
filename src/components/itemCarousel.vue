<template>
  <div>
    <div ref="fItem">
      <div>Hello</div>
      <div>World</div>
    </div>
  </div>
</template>

<script>
import Flickity from "flickity";
export default {
  name: "itemCarousel",
  data() {
    return {
      flickityItem: null,
    };
  },
  mounted() {
    console.log(this.$refs.fItem);
    this.flickity = new Flickity(this.$refs.fItem);
  },
};
</script>
<