<script>
export default {
  data() {
    return {};
  },
};
</script>

<template>
  <!--Newsletter Signup Section-->
  <section class="col-12 col-s-12 newsletter-signup">
    <h2 class="col-6 col-s-6">
      Would you like to see more tips and tutorials on web development?
    </h2>
    <form class="col-6 col-s-6 newsletter-signup-form">
      <label for="firstname">First Name:</label><br />
      <input type="text" id="firstname" />
      <br />
      <label for="lastname">Last Name:</label><br />
      <input type="text" id="lastname" />
      <br />
      <label for="email">Enter your email:</label><br />
      <input type="email" id="email" name="email" />
      <button type="submit">Submit</button>
    </form>
  </section>
</template>

<style></style>
