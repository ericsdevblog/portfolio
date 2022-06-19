<script>
export default {
  data() {
    return {
      skills: [
        { id: 1, name: "HTML & CSS", percentage: "100" },
        { id: 2, name: "JavaScript", percentage: "90" },
        { id: 3, name: "Laravel", percentage: "80" },
        { id: 4, name: "Django", percentage: "70" },
      ],
    };
  },
};
</script>

<template>
  <!--Skills Section-->
  <section class="col-12 col-s-12 skills-section">
    <h2 class="col-12 col-s-12">My Skills</h2>
    <ul class="col-8 col-s-8 skills-list">
      <li v-for="skill in skills" v-bind:key="skill.id">
        {{ skill.name }} - {{ skill.percentage }}
      </li>
    </ul>
  </section>
</template>

<style></style>
