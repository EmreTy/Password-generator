<template>
  <header class="header">
    <div>
      <PasswordGenerator />
    </div>
  </header>
  <main></main>
</template>

<script>
import PasswordGenerator from "./components/PasswordGenerator.vue";

export default {
  name: "App",
  components: {
    PasswordGenerator,
  },
};
</script>

<style>
#app {
}
</style>
