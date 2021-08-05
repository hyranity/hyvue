<template>
  <div class="playgroundComponent">Playground Component</div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  setup() {},
});
</script>

<style lang="scss" scoped>
.playgroundComponent {
  background-color: lightgray;
  padding: 10px;
  border-radius: 4px;
  font-weight: 700;
}
</style>
