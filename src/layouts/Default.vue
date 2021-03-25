<template>
  <div class="layout">
    <topNav></topNav>
    <main class="page__container">
      <slot />
    </main>
    <mainFooter> </mainFooter>
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>
<script>
import topNav from "@/components/topNav.vue";
import mainFooter from "@/components/mainFooter.vue";
export default {
  name: "DefaultLayout",
  components: {
    mainFooter,
    topNav,
  },
};
</script>
<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body {
  background: #1c1a1a;
  font-family: -apple-system, system-ui, BlinkMacSystemFont, "Segoe UI", Roboto,
    "Helvetica Neue", Arial, sans-serif;
  margin: 0;
  padding: 0;
  line-height: 1.5;
}

.header {
  background: rgb(155, 155, 155);
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
  height: 80px;
}
</style>
