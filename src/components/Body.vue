<template>
  <div class="description">
    <h1 class="text">Joel Camacho</h1>
    <h2 class="text">Junior Full-stack Web Developer</h2>
  </div>
</template>

<script>
// import Foo from 'bar/foo'

export default {
  name: "description",
  mixins: [],
  components: {},
  props: {},
  data() {
    return {};
  }
};
</script>

<style  scoped>
.description {
  display: flex;
  flex-direction: column;
  justify-content: center;
  font-family: "Merriweather", serif;
  font-weight: bold;
  font-size: x-large;
  height: 100%;
}
.text {
  color: white;
  margin: 1%;
}
</style>