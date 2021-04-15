<template>
  <div class="serviceAreas__container">
    <h3>MWM Provides services to these States</h3>
    <ul>
      <li>Wisconsin</li>
      <li>Minnesota</li>
      <li>Illinois</li>
      <li>Indiana</li>
      <li>And More...</li>
    </ul>
  </div>
</template>
<script>
export default {
  name: "serviceAreas",
};
</script>

<style scoped>
.serviceAreas__container {
  background: #1c1a1a;
  text-align: center;
  padding: 2.8em;
}
.serviceAreas__container h3 {
  font-size: 28px;
  padding: 8px 12px;
  color: #c32227;
}
.serviceAreas__container ul {
  padding-left: 0;
  list-style: none;
}
.serviceAreas__container ul li {
  color: #d3d3d3;
  font-size: 18px;
  font-weight: 300;
  display: inline-block;
  padding: 4px 14px;
}
</style>