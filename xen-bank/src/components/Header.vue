<template>
  <header>
    <div class="hero-container-header">
      <div class="site-name-logo">
        <h3>{{ logoName }}</h3>
      </div>
      <div class="hero-container-cta">
        <a href="#">
          <button>{{ buttonText }}</button></a
        >
      </div>
    </div>
    <hr />
  </header>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      logoName: "Xen Bank",
      buttonText: "Join the Waiting List",
    };
  },
};
</script>

<style>
.hero-container {
  width: 100%;
  margin-top: -2em;
}
.hero-container-header {
  width: 100%;
  padding: 1em 1em 1em 1em;
  display: flex;
  display: -webkit-flex;
  display: -ms-flexbox;
  -ms-flex-pack: space-between;
  -webkit-box-pack: space-between;
  justify-content: space-between;
  position: relative;
}
.site-name-logo {
  color: var(--text-color);
  font-size: 1em;
  font-weight: 500;
  text-align: left;
  margin: auto 0;
}
hr {
  background-color: var(--text-color);
  height: 1px;
  width: 94%;
  padding: 0 1em;
  margin: 0 auto;
}
.main-hero-section {
  margin: 2em auto;
  padding: 2em 1em;
  display: grid;
  width: 100%;
  grid-template-columns: repeat(auto-fit, minmax(22rem, 1fr));
  grid-gap: 2em;
}
.hero-col-1 h1 {
  font-size: 2em;
  text-align: left;
  padding: 0.2em 0.4em 0.2em 0.4em;
  font-family: var(--font-1);
}
.hero-col-1 p {
  font-size: 0.9em;
  font-family: var(--font-3);
  text-align: justify;
  padding: 0.2em 0.6em 0.2em 0.6em;
  color: var(--text-color);
  font-weight: 500;
  margin: 0em auto 1em auto;
  line-height: 1.5em;
}
.hero-col-2 {
  background-color: rgba(255, 255, 255, 0.1);
  padding: 4em 2em 4em 2em;
  border: solid 2px transparent;
  background-clip: padding-box;
  box-shadow: 10px 10px 10px rgba(46, 54, 68, 0.03);
  backdrop-filter: blur(5px);
  border-radius: 20px;
}
</style>
