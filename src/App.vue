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
  font-family: "Arvo", serif;
  text-align: center;
}

h1 {
  color: #2292a4;
  margin: 20px;
}
body {
  background-color: #0f0a0a;
}

button {
  padding: 15px;
  margin-top: 1.5rem;
  color: black;
  background-color: #2292a4;
}

#password-field {
  background-color: rgb(63, 62, 62);
  color: #f5efed;
  padding: 5px;
  margin-top: 4rem;
}
</style>
