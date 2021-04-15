<template>
  <div class="megaMenu__container">
    <div class="megaMenu__nav">
      <mwm-logo :scrolled="scrolled"></mwm-logo>
      <div class="productItem">Products</div>
      <div class="servicesItem">Services</div>
      <div>Galleries</div>
      <div>Vendors</div>
    </div>
  </div>
</template>
<script>
import mwmLogo from "@/components/mwm-logo.vue";

export default {
  name: "megaMenu",
  props: ["scrolled"],
  components: {
    mwmLogo,
  },
};
</script>
<style>
.megaMenu__container {
  position: fixed;
  width: 100%;
  max-width: 1080px;
  top: 34px;
  z-index: 200;
}
.megaMenu__nav {
  display: flex;
  position: relative;
}
.megaMenu__nav div {
  background: #000;
  display: inline-block;
  width: 25%;
  text-align: center;
  padding-top: 16px;
  padding-bottom: 11px;
  color: white;
  font-weight: 700;
}
.megaMenu__nav div .productMega,
.megaMenu__nav div .servicesMega {
  display: none;
  z-index: 120;
}
.megaMenu__nav div.productItem:hover .productMega,
.megaMenu__nav div.servicesItem:hover .servicesMega {
  display: block;
  position: absolute;
  top: 51px;
  left: 0;
  width: 100%;
}
</style>