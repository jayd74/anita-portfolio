<template>
  <Layout>
    <Hero />
    <!-- <Projects /> -->
  </Layout>
</template>

<script>
import Hero from "~/components/Hero.vue";
export default {
  metaInfo: {
    title: "Hi, I'm Anita Ngo!",
  },
  components: {
    Hero,
  },
};
</script>

<style>
.home-links a {
  margin-right: 1rem;
}
</style>
