<template>
  <div class="skills">
    <h1 v-once>{{name}}</h1>
    {{ btnState ? 'The button is disabled' : 'The button is active'}}
    <button
      v-on:click="changeName"
      v-bind:disabled="btnState"
    >Change Name</button>

    <div class="skills">
      <div class="holder">
        <ul>
          <li v-for="(data, index) in skills" :key="index">{{index}}. {{data.skill}}</li>
        </ul>

        <p v-if="skills.length >= 1">You have more than 1 skill</p>
        <p v-else>You have less than or equal to 1 skill</p>

        <div v-bind:class="{alert: showAlert}"></div>
        <div v-bind:class="alertObject"></div>
      </div>
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
      }
    };
  },
  props: {}
};
</script>

<style scoped>
.alert {
  background-color: yellow;
  width: 100%;
  height: 30px;
  margin-bottom: 30px;
}
</style>
