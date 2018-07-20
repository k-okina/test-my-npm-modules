<template>
  <div id="app">
    HelloWorldContainer開始
    <HelloWorldContainer />
    HelloWorldContainer終了
  </div>
</template>

<script>
import connect from "vue-connect";
import HelloWorld from "./components/HelloWorld.vue";

const HelloWorldContainer = connect({ msg: "helloworld" })(HelloWorld);

export default {
  name: "app",
  components: {
    HelloWorldContainer
  }
};
</script>
