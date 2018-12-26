<template>
  <div class="skills">
    {{ name }}
    <button v-on:click="changeName" v-bind:disabled="btnState">Change Name</button>
  </div>
</template>

<script>
export default {
  name: 'Skills',
  data() {
    return {
      name: 'kdevsoftware',
      btnState: true
    }
  },
  props: {
  }
}
</script>
