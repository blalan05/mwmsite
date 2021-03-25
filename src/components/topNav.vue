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
      <ul class="topNav__container">
        <li class="logoCon">
          <object>
            <svg
              xmlns="http://www.w3.org/2000/svg"
              xmlns:xlink="http://www.w3.org/1999/xlink"
              viewBox="0 0 175.1 78.02"
              style="width: 15%"
            >
              <defs>
                <linearGradient
                  id="New_Gradient_Swatch_2"
                  x1="87.3"
                  y1="-19.66"
                  x2="88.98"
                  y2="78.14"
                  gradientUnits="userSpaceOnUse"
                >
                  <stop offset="0" stop-color="#b9bbbd" />
                  <stop offset="0.05" stop-color="#cacccd" />
                  <stop offset="0.14" stop-color="#e7e8e9" />
                  <stop offset="0.21" stop-color="#f9f9f9" />
                  <stop offset="0.27" stop-color="#fff" />
                  <stop offset="0.42" stop-color="#cccdce" />
                  <stop offset="0.61" stop-color="#929497" />
                  <stop offset="0.64" stop-color="#989a9c" />
                  <stop offset="0.69" stop-color="#a8aaac" />
                  <stop offset="0.74" stop-color="#c2c4c6" />
                  <stop offset="0.8" stop-color="#e6e7e8" />
                  <stop offset="1" stop-color="#6d6e70" />
                </linearGradient>
                <linearGradient
                  id="New_Gradient_Swatch_2-2"
                  x1="35.62"
                  y1="-18.82"
                  x2="37.3"
                  y2="78.99"
                  xlink:href="#New_Gradient_Swatch_2"
                />
                <linearGradient
                  id="New_Gradient_Swatch_2-3"
                  x1="136"
                  y1="-20.46"
                  x2="137.68"
                  y2="77.34"
                  xlink:href="#New_Gradient_Swatch_2"
                />
                <linearGradient
                  id="New_Gradient_Swatch_2-4"
                  x1="132.19"
                  y1="0.92"
                  x2="133.15"
                  y2="56.76"
                  xlink:href="#New_Gradient_Swatch_2"
                />
                <linearGradient
                  id="New_Gradient_Swatch_2-5"
                  x1="31.8"
                  y1="1.86"
                  x2="32.75"
                  y2="57.7"
                  xlink:href="#New_Gradient_Swatch_2"
                />
              </defs>
              <g id="Layer_2" data-name="Layer 2">
                <g id="Layer_1-2" data-name="Layer 1">
                  <path
                    d="M57.76.38,68.31,39.93,81.31.38H94l13,39.55L117.53.38h16.65L115.91,61.61H99.66l-12-35.49-12,35.49H59.38L41.11.38Z"
                    style="fill: url(#New_Gradient_Swatch_2)"
                  />
                  <polyline
                    points="134.18 0.38 115.91 61.61 99.66 61.61"
                    style="
                      fill: none;
                      stroke: #231f20;
                      stroke-miterlimit: 10;
                      stroke-width: 0.75px;
                    "
                  />
                  <polyline
                    points="87.64 26.12 75.62 61.61 59.38 61.61"
                    style="
                      fill: none;
                      stroke: #231f20;
                      stroke-miterlimit: 10;
                      stroke-width: 0.75px;
                    "
                  />
                  <line
                    x1="93.98"
                    y1="0.38"
                    x2="106.97"
                    y2="39.93"
                    style="
                      fill: none;
                      stroke: #231f20;
                      stroke-miterlimit: 10;
                      stroke-width: 0.75px;
                    "
                  />
                  <line
                    x1="57.76"
                    y1="0.38"
                    x2="68.31"
                    y2="39.93"
                    style="
                      fill: none;
                      stroke: #231f20;
                      stroke-miterlimit: 10;
                      stroke-width: 0.75px;
                    "
                  />
                  <line
                    x1="99.66"
                    y1="61.61"
                    x2="87.64"
                    y2="26.12"
                    style="
                      fill: none;
                      stroke: #d0d2d3;
                      stroke-miterlimit: 10;
                      stroke-width: 0.75px;
                    "
                  />
                  <polyline
                    points="106.97 39.93 117.53 0.38 134.18 0.38"
                    style="
                      fill: none;
                      stroke: #d0d2d3;
                      stroke-miterlimit: 10;
                      stroke-width: 0.75px;
                    "
                  />
                  <polyline
                    points="93.98 0.38 81.31 0.38 68.31 39.93"
                    style="
                      fill: none;
                      stroke: #d0d2d3;
                      stroke-miterlimit: 10;
                      stroke-width: 0.75px;
                    "
                  />
                  <polyline
                    points="59.38 61.61 41.11 0.38 57.76 0.38"
                    style="
                      fill: none;
                      stroke: #d0d2d3;
                      stroke-miterlimit: 10;
                      stroke-width: 0.75px;
                    "
                  />
                  <path
                    d="M61,77.64,52.6,46.27,42.3,77.64h-10L21.94,46.27,13.57,77.64H.36L14.85,29.07H27.74l9.53,28.15,9.54-28.15H59.69L74.18,77.64Z"
                    style="fill: url(#New_Gradient_Swatch_2-2)"
                  />
                  <path
                    d="M161.39,77.64,153,46.27l-10.3,31.37H132.66L122.35,46.27,114,77.64H100.77l14.49-48.57h12.89l9.53,28.15,9.54-28.15H160.1l14.49,48.57Z"
                    style="fill: url(#New_Gradient_Swatch_2-3)"
                  />
                  <polyline
                    points="161.39 77.64 174.59 77.64 160.1 29.07"
                    style="
                      fill: none;
                      stroke: #231f20;
                      stroke-miterlimit: 10;
                      stroke-width: 0.75px;
                    "
                  />
                  <polyline
                    points="153.01 46.27 142.71 77.64 132.66 77.64"
                    style="
                      fill: none;
                      stroke: #231f20;
                      stroke-miterlimit: 10;
                      stroke-width: 0.75px;
                    "
                  />
                  <line
                    x1="128.15"
                    y1="29.07"
                    x2="137.68"
                    y2="57.22"
                    style="
                      stroke: #231f20;
                      stroke-miterlimit: 10;
                      stroke-width: 0.75px;
                      fill: url(#New_Gradient_Swatch_2-4);
                    "
                  />
                  <line
                    x1="153.01"
                    y1="46.27"
                    x2="161.39"
                    y2="77.64"
                    style="
                      fill: none;
                      stroke: #e6e7e8;
                      stroke-miterlimit: 10;
                      stroke-width: 0.75px;
                    "
                  />
                  <polyline
                    points="160.1 29.07 147.22 29.07 137.68 57.22"
                    style="
                      fill: none;
                      stroke: #e6e7e8;
                      stroke-miterlimit: 10;
                      stroke-width: 0.75px;
                    "
                  />
                  <line
                    x1="122.35"
                    y1="46.27"
                    x2="132.66"
                    y2="77.64"
                    style="
                      fill: none;
                      stroke: #e6e7e8;
                      stroke-miterlimit: 10;
                      stroke-width: 0.75px;
                    "
                  />
                  <polyline
                    points="100.77 77.64 115.26 29.07 127.77 29.07"
                    style="
                      fill: none;
                      stroke: #e6e7e8;
                      stroke-miterlimit: 10;
                      stroke-width: 0.75px;
                    "
                  />
                  <polyline
                    points="100.77 77.64 113.97 77.64 122.35 46.27"
                    style="
                      fill: none;
                      stroke: #231f20;
                      stroke-miterlimit: 10;
                      stroke-width: 0.75px;
                    "
                  />
                  <line
                    x1="37.27"
                    y1="57.22"
                    x2="27.74"
                    y2="29.07"
                    style="
                      stroke: #231f20;
                      stroke-miterlimit: 10;
                      stroke-width: 0.75px;
                      fill: url(#New_Gradient_Swatch_2-5);
                    "
                  />
                  <polyline
                    points="0.36 77.64 13.57 77.64 21.94 46.27"
                    style="
                      fill: none;
                      stroke: #231f20;
                      stroke-miterlimit: 10;
                      stroke-width: 0.75px;
                    "
                  />
                  <polyline
                    points="32.25 77.64 42.3 77.64 52.6 46.27"
                    style="
                      fill: none;
                      stroke: #231f20;
                      stroke-miterlimit: 10;
                      stroke-width: 0.75px;
                    "
                  />
                  <polyline
                    points="60.98 77.64 74.19 77.64 59.69 29.07"
                    style="
                      fill: none;
                      stroke: #231f20;
                      stroke-miterlimit: 10;
                      stroke-width: 0.75px;
                    "
                  />
                  <polyline
                    points="0.36 77.64 14.85 29.07 27.74 29.07"
                    style="
                      fill: none;
                      stroke: #e6e7e8;
                      stroke-miterlimit: 10;
                      stroke-width: 0.75px;
                    "
                  />
                  <line
                    x1="21.94"
                    y1="46.27"
                    x2="32.25"
                    y2="77.64"
                    style="
                      fill: none;
                      stroke: #e6e7e8;
                      stroke-miterlimit: 10;
                      stroke-width: 0.75px;
                    "
                  />
                  <polyline
                    points="37.27 57.22 46.81 29.07 59.69 29.07"
                    style="
                      fill: none;
                      stroke: #e6e7e8;
                      stroke-miterlimit: 10;
                      stroke-width: 0.75px;
                    "
                  />
                  <line
                    x1="52.6"
                    y1="46.27"
                    x2="60.98"
                    y2="77.64"
                    style="
                      fill: none;
                      stroke: #e6e7e8;
                      stroke-miterlimit: 10;
                      stroke-width: 0.75px;
                    "
                  />
                </g>
              </g>
            </svg>
          </object>
        </li>
        <template v-for="(item, i) in menuItems">
          <g-link :to="item.route" :key="i">
            <li>{{ item.text }}</li>
          </g-link>
        </template>
      </ul>
    </template>
  </nav>
</template>

<script>
export default {
  name: "topNav",
  data() {
    return {
      toggleOCN: false,
      menuItems: [
        { text: "(920) 927-3851", route: "tel:9209273851" },
        { text: "info@mgrf.com", route: "mailto:info@mgrf.com" },
        { text: "About", route: "/about" },
        { text: "Contact", route: "/contact" },
        { text: "Careers", route: "/careers" },
      ],
      windowWidth: window.innerWidth,
    };
  },
  mounted() {
    window.addEventListener("resize", this.onResize);
  },
  methods: {
    onResize() {
      this.windowWidth = window.innerWidth;
    },
  },
  beforeDestroy() {
    window.removeEventListener("onresize", this.onResize);
  },
};
</script>

<style>
.topNav__container {
  background: #ff0000;
  /* border-bottom: 3px solid red; */
  display: flex;
  justify-content: space-around;
}
.topNav__container li {
  list-style: none;
  padding: 5px 18px;
}
.topNav__container a {
  color: rgb(255, 255, 255);
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