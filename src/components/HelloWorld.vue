<template>
  <div class="hello">
    <div class="title">
      <img alt="Vue logo" src="../assets/logo.png" />
    </div>
    <h1>{{ msg }}</h1>
    <p>
      This is a VueJS boilerplate developed by Hyranity. For additional
      information, please see
      <a href="https://cli.vuejs.org" target="_blank" rel="noopener"
        >vue-cli documentation</a
      >.
    </p>
    <PlaygroundVue />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import PlaygroundVue from "./Playground.vue";

export default defineComponent({
  setup() {},
  data() {
    return { msg: "HyVue Boilerplate" };
  },
  components: {
    PlaygroundVue,
  },
});
</script>



<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
.hello {
  margin: 0;
  padding: 0;
  & .title {
    background-color: #d8e3d8;
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 15px;

    & img {
      height: 50px;
      margin-right: 20px;
    }

    & h1 {
      margin: 0;
    }
  }
}
</style>
