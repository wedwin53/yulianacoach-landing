<template>
  <div class="hello">
    <h1 class="title-text">{{ msg }}</h1>

    <p class="welcome-text">
      Nos encontramos creando un producto maravilloso para mejorar tu calidad de
      vida!
    </p>
    <br />
     <vue-calendly url="https://calendly.com/yuliana-4/60min" :height="600"></vue-calendly>
    <p class="text-newsletter">
      Suscribase a nuestra lista para recursos y lanzamientos
    </p>
  </div>
</template>

<script>
import Vue from 'vue';
import VueCalendly from 'vue-calendly';
Vue.use(VueCalendly);

export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hello {
  margin-top: 10px;
  border-radius: 5px;
  padding: 10px;
  background-color: rgba(255, 255, 255, 0.7);
  box-shadow: rgba(29, 22, 22, 0.5) 4px 2px 2px;
}

h1 {
  margin: 40px 0 0;
  font-size: 40px;
  color: black;
  text-shadow: rgba(77, 76, 74, 0.5) 10px 10px 10px;
}

.welcome-text {
  font-size: 25px;
  font-weight: 300;
  color: black;
}

.text-newsletter {
  color: black;
  font-size: 25px;
  font-weight: 300;
}
</style>
