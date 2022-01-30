<template>
  <section class="hero-container">
    <Header />
    <div class="main-hero-section">
      <div class="hero-col-1">
        <h1>{{ headertext }}</h1>
        <p>{{ headerparagraph }}</p>
      </div>
      <div class="hero-col-2">
        <SignUpForm />
        <iconSvg />
      </div>
    </div>
  </section>
  <service />
  <section class="info-section">
    <div class="main-hero-section">
      <div class="hero-col-1">
        <h2>{{ infoHead }}</h2>
        <p>{{ infoText }}</p>
      </div>
      <div class="hero-col-2">
        <SignUpForm />
      </div>
    </div>
  </section>
  <Footer />
</template>

<script>
import Header from "./components/Header.vue";
import SignUpForm from "./components/SignUpForm.vue";
import service from "./components/service.vue";
import Footer from "./components/Footer.vue";
import iconSvg from "./components/iconSvg.vue";
export default {
  name: "App",
  components: {
    Header,
    SignUpForm,
    service,
    Footer,
    iconSvg,
  },
  data() {
    return {
      headertext: "Welcome to the world of Decentralized Banking",
      headerparagraph: "Do everything the traditional bank can do and more",
      infoHead: "Get Early Access",
      infoText:
        "We are on track to being the biggest decentralized bank in the world and joining the waiting list means a lot of benefit for you too.",
    };
  },
};
</script>

<style>
#app {
  font-family: "Raleway", sans-serif;
  font-family: "Lato", sans-serif;
  font-family: "Lato", sans-serif;
  font-family: "Raleway", sans-serif;
}
.info-section h2 {
  font-size: 2em;
  text-align: center;
  padding: 0.2em 0.4em 0.2em 0.4em;
  font-family: var(--font-1);
  color: var(--text-color);
}

.info-section p {
  font-size: 0.9em;
  font-family: var(--font-3);
  text-align: center;
  padding: 0.2em 1em 0.2em 1em;
  color: var(--text-color);
  font-weight: 500;
  margin: 0em auto 1em auto;
  line-height: 1.5em;
}
</style>
