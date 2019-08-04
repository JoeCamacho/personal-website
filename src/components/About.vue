<template>
  <div class="about">
    <div class="about-description">
      <h2>Who I'm?</h2>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Soluta alias aut obcaecati deserunt debitis eos nisi, eveniet assumenda consequuntur! Aliquam modi odio enim, repudiandae cum tenetur voluptates delectus quibusdam rerum!</p>
    </div>
    <div class="about-skills">
      <h2>Skills</h2>
      <div class="about-grid">
        <aside class="about-grid-item">
          <h3>Front-end</h3>
          <ul class="about-list">
            <li>HTML / CSS</li>
            <li>JavaScript</li>
            <li>React</li>
            <li>Vue.js</li>
          </ul>
        </aside>

        <article class="about-grid-item">
          <h3>Back-end</h3>
          <ul class="about-list">
            <li>Node.js</li>
            <li>Express.js</li>
          </ul>
        </article>

        <aside class="about-grid-item">
          <h3>DataBase</h3>
          <ul class="about-list">
            <li>Postgresql</li>
            <li>MondoDB</li>
          </ul>
        </aside>
        <footer>
          <h3>Other tools</h3>
          <ul class="about-list2">
            <li class="about-list2-item">Git / GitHub / Bash</li>
            <li class="about-list2-item">Command Line Interface</li>
            <li class="about-list2-item">Trello</li>
            <li class="about-list2-item">Slack</li>
            <li class="about-list2-item">VS Code</li>
          </ul>
        </footer>
      </div>
    </div>
    <div class="btn btn-one">
      <span>Contact me</span>
    </div>
  </div>
</template>

<script>
// import Foo from 'bar/foo'

export default {
  name: "about",
  mixins: [],
  components: {},
  props: {},
  data() {
    return {};
  }
};
</script>

<style  scoped>
.about {
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  background-color: white;
  color: #049e75;
}

.about-description {
  max-width: 80%;
}
.about-skills {
  justify-content: center;
  width: 100%;
}

.about-grid {
  display: grid;
  justify-content: center;
  grid-template-columns: 30% 30% 30%;
  grid-template-rows: repeat(1, 300px);
  grid-gap: 1em;
}
.about-grid-item {
  flex-direction: column;
  justify-content: center;
  font-size: larger;
}

aside,
article,
footer {
  background: #eaeaea;
  padding: 1em;
  border: solid 1px #00b787;
}

body {
  margin: 0 auto;
  max-width: 56em;
  padding: 1em 0;
}

.grid > * {
  display: flex;
  align-items: center;
  justify-content: center;
}
header,
footer {
  grid-column: 1 / 4;
}

.about-list {
  list-style-type: none;
  margin: 0;
  padding: 0;
}
.about-list2 {
  display: flex;
  flex-direction: row;
  justify-content: center;
  list-style-type: none;
  margin: 0 10% 0 10%;
  font-size: larger;
}
.about-list2-item {
  padding-right: 30px;
}

.btn-one {
  padding: 0 2% 0 2%;
  margin: 5% 10% 5% 10%;
  max-width: 150px;
  color: #00b787;
  transition: all 0.3s;
  position: relative;
  font-size: x-large;
  font-weight: bolder;
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
  border-top-color: #00b787;
  border-bottom-color: #00b787;
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