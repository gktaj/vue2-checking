<template>
  <div class="skills">
    <h1 v-once>{{name}}</h1>
    {{ btnState ? 'The button is disabled' : 'The button is active'}}
    <button
      v-on:click="changeName"
      v-bind:disabled="btnState"
    >Change Name</button>
  </div>
</template>

<script>
export default {
  name: "Skills",
  data() {
    return {
      name: "kdevsoftware",
      btnState: true
    };
  },
  props: {}
};
</script>
