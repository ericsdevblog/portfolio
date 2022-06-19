<script>
import ProjectComponent from "@/components/ProjectComponent.vue";
export default {
  data() {
    return {
      posts: [
        {
          id: 1,
          content:
            "This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.",
          image: "/images/p1.jpg",
        },
        {
          id: 2,
          content:
            "This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.",
          image: "/images/p2.jpg",
        },
        {
          id: 3,
          content:
            "This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.",
          image: "/images/p3.jpg",
        },
        {
          id: 4,
          content:
            "This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.",
          image: "/images/p3.jpg",
        },
        {
          id: 5,
          content:
            "This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.",
          image: "/images/p2.jpg",
        },
        {
          id: 6,
          content:
            "This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.",
          image: "/images/p1.jpg",
        },
      ],
    };
  },
  components: { ProjectComponent },
};
</script>

<template>
  <!--Projects Section-->
  <section class="col-12 col-s-12 porject-section" id="project">
    <h2 class="col-12 col-s-12">My Projects</h2>
    <ProjectComponent
      v-for="post in posts"
      v-bind:content="post.content"
      v-bind:image="post.image"
      v-bind:key="post.id"
    ></ProjectComponent>
  </section>
</template>

<style></style>
