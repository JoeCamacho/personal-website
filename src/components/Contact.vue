<template>
  <div class="contact">
    <div class="contact-box">
      <div class="btn btn-one">
        <span>GitHub</span>
      </div>
      <div class="btn btn-one">
        <span>LinkedIn</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "contact",
  mixins: [],
  components: {},
  props: {},
  data() {
    return {};
  }
};
</script>

<style  scoped>
.contact {
  font-family: "Montserrat", sans-serif;
  height: 15%;
}

.contact-box {
  display: flex;
  flex-direction: row;
  justify-content: center;
}

.btn-one {
  padding: 0 2% 0 2%;
  margin: 0 5% 0 5%;
  max-width: 120px;
  color: #fff;
  transition: all 0.3s;
  position: relative;
  font-size: large;
}
.btn-one span {
  transition: all 0.3s;
}
.btn-one::before {
  content: "";
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: 1;
  opacity: 0;
  transition: all 0.3s;
  border-top-width: 1px;
  border-bottom-width: 1px;
  border-top-style: solid;
  border-bottom-style: solid;
  border-top-color: rgba(255, 255, 255, 0.5);
  border-bottom-color: rgba(255, 255, 255, 0.5);
  transform: scale(0.1, 1);
}
.btn-one:hover span {
  letter-spacing: 2px;
}
.btn-one:hover::before {
  opacity: 1;
  transform: scale(1, 1);
}
.btn-one::after {
  content: "";
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: 1;
  transition: all 0.3s;
  background-color: rgba(255, 255, 255, 0.1);
}
.btn-one:hover::after {
  opacity: 0;
  transform: scale(0.1, 1);
}
</style>
