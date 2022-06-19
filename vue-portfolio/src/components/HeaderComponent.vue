<script>
export default {
  data() {
    return {
      navLinks: [
        { id: 1, name: "Home", link: "#" },
        { id: 2, name: "Features", link: "#" },
        { id: 3, name: "Pricing", link: "#" },
        { id: 4, name: "FAQs", link: "#" },
        { id: 5, name: "About", link: "#" },
      ],
    };
  },

  props: ["websiteName"],
};
</script>

<template>
  <!--Header and Navigation Bar-->
  <div class="col-12 col-s-12 header-and-nav">
    <header class="col-4 col-s-4 header">
      <h1>{{ websiteName }}</h1>
    </header>
    <nav class="col-8 col-s-8">
      <ul class="nav-list">
        <li
          class="nav-item"
          v-for="navLink in navLinks"
          v-bind:key="navLink.id"
        >
          <a href="/portfolio.html" v-bind:href="navLink.link">{{
            navLink.name
          }}</a>
        </li>
      </ul>
    </nav>
  </div>
</template>

<style></style>
