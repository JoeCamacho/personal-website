<template>
  <div class="about-page">
    <About />
  </div>
</template>

<script>
import About from "@/components/About.vue";

export default {
  name: "about-page",
  mixins: [],
  components: {
    About
  },
  props: {},
  data() {
    return {};
  }
};
</script>

<style  scoped>
.about-page {
  margin: 0 auto;
  height: 100%;
  width: 90%;
}
</style>
