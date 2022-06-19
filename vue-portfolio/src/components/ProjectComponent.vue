<script>
export default {
  props: ["content", "image"],
};
</script>

<template>
  <div class="col-4 col-s-4">
    <div class="project-card">
      <h3>My Project</h3>
      <img :src="image" />
      <p>{{ content }}</p>
    </div>
  </div>
</template>

<style></style>
