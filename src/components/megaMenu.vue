<template>
  <div class="megaMenu__container">
    <ul class="megaMenu__nav">
      <li class="productItem">
        Products
        <div class="productMega">
          <div>
            <ul>
              <li>
                400 Feed Body
                <ul>
                  <li>About</li>
                  <li>Description</li>
                  <li>Options</li>
                </ul>
              </li>
              <li>
                4034 Feed Body
                <ul>
                  <li>About</li>
                  <li>Description</li>
                  <li>Options</li>
                </ul>
              </li>
              <li>
                5012 Feed Body
                <ul>
                  <li>About</li>
                  <li>Descriptions</li>
                  <li>Options</li>
                </ul>
              </li>
            </ul>
          </div>
        </div>
      </li>
      <li class="servicesItem">
        Services
        <div class="servicesMega">
          <div>
            <ul>
              <li>Feed Body Repairs</li>
              <li>Manufacturing/Welding</li>
              <li>Road Crew/Millwrights</li>
              <li>Machine Shop</li>
              <li>Waterjet</li>
              <li>Drafting</li>
              <li>Sandblasting</li>
              <li>Painting</li>
              <li>Hot-dipped Galvanized</li>
              <li>Truck Repairs</li>
              <li>Buy Parts</li>
              <li>Advising/Consulting</li>
            </ul>
          </div>
        </div>
      </li>
      <li>Galleries</li>
      <li>Vendors</li>
    </ul>
    <div></div>
  </div>
</template>
<script>
export default {
  name: "megaMenu",
};
</script>
<style>
.megaMenu__nav {
  display: flex;
  position: relative;
}
.megaMenu__nav li {
  background: #0000ff;
  display: inline-block;
  width: 25%;
  text-align: center;
  padding-top: 16px;
  padding-bottom: 11px;
  color: white;
  font-weight: 700;
}
.megaMenu__nav li:hover {
  background: #0000aa;
}
.megaMenu__nav li .productMega,
.megaMenu__nav li .servicesMega {
  display: none;
  z-index: 120;
}
.megaMenu__nav li.productItem:hover .productMega,
.megaMenu__nav li.servicesItem:hover .servicesMega {
  display: block;
  position: absolute;
  top: 51px;
  left: 0;
  width: 100%;
}
.megaMenu__nav li.productItem .productMega div,
.megaMenu__nav li.productItem .productMega div {
  width: 100%;
  display: inline-block;
}
.megaMenu__nav li.productItem .productMega div ul,
.megaMenu__nav li.servicesItem .servicesMega div ul {
  width: 100%;
}
.megaMenu__nav li.productItem .productMega div ul li,
.megaMenu__nav li.servicesItem .servicesMega div ul li {
  width: 33.33%;
}
.megaMenu__nav li.productItem .productMega div ul li ul,
.megaMenu__nav li.servicesItem .servicesMega div ul li ul {
  width: 100%;
}
.megaMenu__nav li.productItem .productMega div ul li ul li,
.megaMenu__nav li.servicesItem .servicesMega div ul li ul li {
  width: 100%;
}
</style>