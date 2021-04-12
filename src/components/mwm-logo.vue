<template>
  <div class="logoCon">
    <g-image
      src="~/assets/SVG/mwm-full.svg"
      alt="Midwest Welding & Manuacturing Logo"
      :class="['full-logo', { 'hide-logo': scrolled > 11 }]"
    />
    <g-image
      src="~/assets/SVG/mwm-bw.svg"
      alt="Midwest Welding & Manuacturing Logo"
      :class="[
        'bw-logo',
        { 'hide-logo': scrolled < 12 },
        { scrolled: scrolled > 11 },
      ]"
    />
  </div>
</template>

<script>
export default {
  name: "MWMLogo",
  props: ["scrolled"],
};
</script>

<style>
.logoCon {
  position: relative;
}
.full-logo,
.bw-logo {
  position: absolute;
  opacity: 1;
  transition: all 0.3s;
  top: -20px;
  width: 75%;
  left: 25%;
}
.bw-logo.scrolled {
  top: -48px;
  width: 50%;
  left: 33%;
}
.hide-logo {
  opacity: 0;
}
</style>