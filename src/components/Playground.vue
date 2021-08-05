<template>
  <div class="playground">
    <h3>{{ title }}</h3>

    <div class="playground__container"><playground-component /></div>
    <p>{{ description }}</p>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import PlaygroundComponent from "./PlaygroundComponent.vue";

export default defineComponent({
  setup() {},
  data() {
    return {
      title: "Component Playground",
      description:
        "Above is a playground where you can test VueJS component designs. Or you can simply remove the page and start your own project.",
    };
  },
  components: { PlaygroundComponent },
});
</script>

<style lang="scss" scoped>
.playground {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  & h3 {
    margin: 0;
    margin-top: 40px;
    margin-bottom: 5px;
  }

  & p {
    padding: 0;
    margin: 0;
    margin-top: 10px;
    opacity: 0.8;
  }
}

.playground__container {
  border: 1px solid grey;
  width: 1000px;
  height: 500px;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
