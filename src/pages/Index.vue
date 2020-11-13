<template>
  <Layout>
    <Hero />
    <Projects />
  </Layout>
</template>

<script>
import Hero from "~/components/Hero.vue";
import Projects from "~/components/Projects.vue";
export default {
  metaInfo: {
    title: "Hi, I'm Anita Ngo!",
  },
  components: {
    Hero,
    Projects,
  },
};
</script>

<style>
.home-links a {
  margin-right: 1rem;
}
</style>
