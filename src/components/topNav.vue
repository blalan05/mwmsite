<template>
  <nav>
    <!-- // Vertical -->
    <template v-if="windowWidth < 720">
      <div class="offCanvasNav__container">
        <button
          @click="toggleOCN = !toggleOCN"
          style="margin: 8px; background: none; color: white; border: none"
        >
          <object>
            <svg viewBox="0 0 100 80" width="40" height="40">
              <rect width="100" height="18" style="fill: white"></rect>
              <rect y="30" width="100" height="18" style="fill: white"></rect>
              <rect y="60" width="100" height="18" style="fill: white"></rect>
            </svg>
          </object>
        </button>
        <ul :class="['offCanvasNav', { onCanvasNav: toggleOCN }]">
          <template v-for="(item, i) in menuItems">
            <g-link :to="item.route" :key="i">
              <li>{{ item.text }}</li>
            </g-link>
          </template>
        </ul>
      </div>
    </template>
    <!-- Horizontal -->
    <template v-else>
      <div class="topNav__container">
        <template v-for="(item, i) in menuItems">
          <g-link :to="item.route" :key="i">
            <span>{{ item.text }}</span>
          </g-link>
        </template>
      </div>
      <mega-menu :scrolled="scrolled"></mega-menu>
    </template>
  </nav>
</template>

<script>
import megaMenu from "../components/megaMenu.vue";

export default {
  name: "topNav",
  props: ["scrolled"],
  data() {
    return {
      toggleOCN: false,
      menuItems: [
        { text: "About", route: "/about" },
        { text: "Contact", route: "/contact" },
        { text: "Careers", route: "/careers" },
        { icon: "fa fa-envelope", route: "mailto:info@mgrf.com" },
        { text: "(920) 927-3851", route: "tel:9209273851" },
      ],
      windowWidth: 0,
    };
  },
  mounted() {
    this.windowWidth = window.innerWidth;
    document.addEventListener("resize", this.onResize);
  },
  methods: {
    onResize() {
      this.windowWidth = window.innerWidth;
    },
  },
  beforeDestroy() {
    document.removeEventListener("onresize", this.onResize);
  },
  components: {
    megaMenu,
  },
};
</script>

<style>
.topNav__container {
  background: #000;
  position: fixed;
  top: 0;
  width: 100%;
  max-width: 1080px;
  display: flex;
  justify-content: flex-end;
}
.topNav__container a {
  padding: 5px 18px;
  color: rgb(211, 211, 211);
  font-weight: 400;
  text-decoration: none;
}
.offCanvasNav {
  background: black;
  position: fixed;
  height: 100vh;
  top: 0;
  bottom: 0;
  width: 80%;
  max-width: 360px;
  left: -360px;
  transition: left 0.4s;
  margin-top: 59px;
  padding: 14px;
}
.offCanvasNav__container {
  background: #ff0000;
}
.offCanvasNav.onCanvasNav {
  left: 0;
}
.offCanvasNav a {
  color: white;
}
.offCanvasNav li {
  list-style: none;
  padding: 10px 12px;
}
</style>