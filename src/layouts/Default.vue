<template>
  <div class="layout">
    <topNav :scrolled="scrolled"></topNav>
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
  data() {
    return {
      scrolled: 0,
    };
  },
  components: {
    mainFooter,
    topNav,
  },
  beforeDestroy() {
    document.removeEventListener("scroll", this.handleScroll);
  },
  mounted() {
    document.addEventListener("scroll", this.handleScroll);
  },
  methods: {
    handleScroll(e) {
      this.scrolled = window.scrollY;
    },
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
  background: #5f5f5f;
  font-family: -apple-system, system-ui, BlinkMacSystemFont, "Segoe UI", Roboto,
    "Helvetica Neue", Arial, sans-serif;
  margin: 0;
  padding: 0;
  line-height: 1.5;
}

.layout {
  max-width: 1080px;
  margin: auto;
  position: relative;
  box-shadow: 0px 0px 4px 2px #1c1a1a;
}

.header {
  background: rgb(155, 155, 155);
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
  height: 80px;
}
.page__container {
  padding-top: 86px;
}
</style>
