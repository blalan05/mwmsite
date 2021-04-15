<template>
  <footer>
    <div class="footer__wrapper">
      <div>
        <div class="footer__contact">
          <h3>Contact</h3>
          <p>Phone: (920) 927-3851</p>
          <p>Fax: (920) 927-5551</p>
        </div>
        <div class="footer__logo">
          <g-image
            src="~/assets/SVG/mwm-full.svg"
            alt="Midwest Welding & Manuacturing Logo"
          />
        </div>
        <div class="footer__address">
          <h3>Address</h3>
          <p>202 Harrison Street</p>
          <p>P.O. Box 39</p>
          <p>Reeseville, WI 53579</p>
        </div>
      </div>
      <div class="footer_row2">
        <div>
          <a href="">Products</a>
          <a href="">Services</a>
          <a href="">Recent Projects</a>
        </div>
        <div>
          <a href="">Request Quote</a>
          <a href="">Services</a>
          <a href="">Careers</a>
        </div>
        <div>
          <a href="">Vendors</a>
          <a href="">About</a>
          <a href="">Contact</a>
        </div>
        <div style="display: inline-block">
          2012 &copy; Copyright Midwest Welding & Manufacturing LLC
        </div>
      </div>
    </div>
  </footer>
</template>
<script>
export default {
  name: "mainFooter",
};
</script>
<style scoped>
footer {
  background: #1c1a1a;
  color: white;
  width: 100%;
  border-top: 3px solid #c32227;
}
footer .footer__wrapper {
  padding: 2.5em;
  box-sizing: border-box;
  width: 100%;
}
footer .footer__logo {
  display: inline-block;
  width: 25%;
}
footer .footer__logo img {
  width: 75%;
}
footer .footer__contact {
  display: inline-block;
  width: 33.33%;
}
footer .footer__address {
  display: inline-block;
  width: 33.33%;
}
footer .footer_row2 {
  width: 100%;
}
footer .footer_row2 a {
  display: block;
  color: #d3d3d3;
  text-decoration: none;
}
footer .footer_row2 div {
  width: 25%;
  padding: 1.8em;
  display: inline-block;
}
</style>