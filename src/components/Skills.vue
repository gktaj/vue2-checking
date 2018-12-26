<template>
  <div class="container">
    <div class="holder">
      <ul>
        <li v-for="(data, index) in skills" :key="index">{{data.skill}}</li>
      </ul>
      <p>These are the skills that you possess.</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Skills",
  data() {
    return {
      name: "kdevsoftware",
      btnState: true,
      skills: [{ skill: "Vue.js" }, { skill: "Frontend Developer" }],
      showAlert: true,
      alertObject: {
        alert: true
      },
      bgColor: "red",
      bgWidth: "100px",
      bgHeight: "200px",
      alertStyle: {
        background: "red",
        width: "100px",
        height: "200px"
      }
    };
  },
  props: {}
};
</script>

<style scoped>
.holder {
  background: #fff;
}

ul {
  margin: 0;
  padding: 0;
  list-style-type: none;
}

ul li {
  padding: 20px;
  font-size: 1.3em;
  background-color: #e0edf4;
  border-left: 5px solid #3eb3f6;
  margin-bottom: 2px;
  color: #3e5252;
}

p {
  text-align: center;
  padding: 30px 0;
  color: gray;
}

.container {
  box-shadow: 0px 0px 40px lightgray;
}
</style>
