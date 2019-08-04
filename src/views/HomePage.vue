<template>
  <div class="home-page">
    <Body />
    <Contact />
  </div>
</template>

<script>
import Body from "@/components/Body.vue";
import Contact from "@/components/Contact.vue";

export default {
  name: "home-page",
  components: {
    Body,
    Contact
  }
};
</script>

<style scoped>
html,
body {
  height: 100%;
}
.home-page {
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
}
</style>
