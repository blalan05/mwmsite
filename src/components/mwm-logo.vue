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
      :class="['bw-logo', { 'hide-logo': scrolled < 12 }]"
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
  top: -20px;
  width: 75%;
  left: 25%;
}
.hide-logo {
  opacity: 0;
}
</style>