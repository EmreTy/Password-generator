<template>
  <section>
    <h1>Password Generator</h1>
    <p id="password-field">PasswordThatWillGenerate</p>
    <button>Copy to Clipboard</button>
    <p id="choose">Choose your Charakter set:</p>
  </section>
  <section>
    <form v-on:submit.prevent="add">
      <input type="checkbox" class="checkboxLowercase" id="checkbox01" />
      <label class="buttonLabel" for="checkbox01">Lowercase</label>
      <input type="checkbox" class="checkboxUppercase" id="checkbox01" />
      <label class="buttonLabel" for="checkbox01">Uppercase</label>
      <input type="checkbox" class="checkboxNumbers" id="checkbox01" />
      <label class="buttonLabel" for="checkbox01">Numbers</label>
      <input type="checkbox" class="checkboxSymbols" id="checkbox01" />
      <label class="buttonLabel" for="checkbox01">Symbols</label>
    </form>
    <form v-on:submit.prevent="add">
      <p id="choose">Password Length:</p>
      <input type="range" class="slider" id="slide123" />
      <label class="sliderLabel" for="slide123" min="8" max="30"></label>
    </form>
  </section>
</template>

<script>
export default {
  name: "PasswordGenerator",
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
  margin: 1.5rem;
  color: black;
  background-color: #2292a4;
}

#password-field {
  background-color: rgb(63, 62, 62);
  color: #f5efed;
  padding: 5px;
  margin-top: 4rem;
}

.checkboxLowercase,
.checkboxUppercase,
.checkboxNumbers,
.checkboxSymbols {
  all: unset;
}
.buttonLabel {
  margin: 1rem;
  padding: 5px;
  border: 0.2rem solid white;
  border-radius: 0.2rem;
  color: white;
}

#choose {
  color: white;
  margin: 2rem;
}
</style>
