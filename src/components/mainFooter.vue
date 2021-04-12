<template>
  <footer>
    <div class="footer__wrapper">
      <div class="footer__logo">
        <g-image
          src="~/assets/SVG/mwm-full.svg"
          alt="Midwest Welding & Manuacturing Logo"
        />
      </div>
      <div class="footer__contact">
        <h3>Contact</h3>
        <p>Phone: (920) 927-3851</p>
        <p>Fax: (920) 927-5551</p>
      </div>
      <div class="footer__address">
        <h3>Address</h3>
        <p>202 Harrison Street</p>
        <p>P.O. Box 39</p>
        <p>Reeseville, WI 53579</p>
      </div>
    </div>
  </footer>
</template>
<script>
export default {
  name: "mainFooter",
};
</script>
<style>
footer {
  background: #1c1a1a;
  color: white;
  width: 100%;
  border-top: 3px solid #c32227;
}
footer .footer__wrapper {
  width: 88%;

  margin: 0 auto;
  padding: 2.5em 0;
}
footer .footer__logo {
  display: inline-block;
  width: 33.33%;
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
</style>