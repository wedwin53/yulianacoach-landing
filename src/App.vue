<template>
  <div id="app">
    <img
      alt="Yuliana Coach Logo"
      class="logo"
      src="./assets/yc-logo-tiny.jpg"
    />
    <HelloWorld msg="Bienvenid@" />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld";

export default {
  name: "App",
  components: {
    HelloWorld,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Ubuntu:wght@300;500;700&display=swap");
#app {
  font-family: "Ubuntu", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

html {
  background-image: url("dominic-dreier-kztP2WFVIXM-unsplash.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  height: 100%;
}

.logo {
  max-width: 60%;
  box-shadow: rgb(105, 101, 101) 5px 10px 15px;
  border-radius: 10px;
}

@media (min-width: 600px) {
  .logo {
    max-width: 25%;
  }
}
</style>
