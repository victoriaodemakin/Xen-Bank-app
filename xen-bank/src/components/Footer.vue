<template>
  <footer>
    <div class="footer-attribution">
      <ul>
        <li><a href="#"> Privacy Policy</a></li>
        <li><a href="#"> FAQs</a></li>
        <li><a href="#"> Terms and Condition</a></li>
      </ul>
    </div>
    <div class="footer-site-name">
      <p>{{ logoName }}</p>
    </div>
  </footer>
</template>
<script>
export default {
  name: "Footer",
  data() {
    return {
      logoName: "XenBank",
    };
  },
};
</script>
<style>
footer {
  width: 100%;
  display: flex;
  justify-content: space-between;
  padding: 0em 1em;
}
.footer-attribution {
  position: relative;
  width: 100%;
}

.footer-site-name p {
  color: var(--text-color);
  font-family: var(--font-3);
  font-size: 0.5em;
  font-weight: 400;
  display: inline;
}
.footer-attribution ul {
  width: 100%;
  list-style-type: none;
  display: flex;
  display: -ms-flexbox;
  display: -webkit-flex;
  justify-content: flex-start;
  align-items: flex-start;
  -webkit-box-align: flex-start;
  flex-direction: row;
  -webkit-box-orient: horizontal;
  -ms-flex-direction: row;
}
.footer-attribution ul li {
  margin: 2px;
}
.footer-attribution ul li a {
  text-decoration: none;
  color: var(--text-color);
  font-family: var(--font-3);
  font-size: 0.5em;
  font-weight: 400;
  text-transform: capitalize;
}
</style>
