<template>
  <section>
    <div class="service__item">
      <h3>Field Service</h3>
      <p>
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Deleniti
        mollitia maxime labore animi aspernatur molestiae!
      </p>
    </div>
    <div class="service__item">
      <h3>Shop Services</h3>
      <p>
        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Saepe ipsum
        exercitationem aliquam facilis illum dolorum!
      </p>
    </div>
    <div class="service__item">
      <h3>Feed Body Services</h3>
      <div class="service__item-body">
        <p>
          Lorem ipsum, dolor sit amet consectetur adipisicing elit. Nulla sint
          aspernatur vero officiis! Aliquam optio.
        </p>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: "Services",
};
</script>

<style scoped>
section {
  width: 100%;
  display: flex;
  background: #1c1a1a;
}
.service__item {
  text-align: center;
  width: 33.33%;
  padding: 48px 24px;
  color: rgb(211, 211, 211);
}
.service__item h3 {
  text-transform: uppercase;
  font-weight: 400;
}
section:first-child {
  padding-left: 48px;
}
section:last-child {
  padding-right: 48px;
}
</style>