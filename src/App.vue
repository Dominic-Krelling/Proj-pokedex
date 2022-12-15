<script lang="ts">
import { defineComponent } from "vue";
import HeaderView from "./components/HeaderView.vue";
import BottomButton from "./components/BottomButton.vue";

export default defineComponent({
  setup() {
    return {};
  },
  components: { HeaderView, BottomButton },
});
</script>
<template>
  <div>
    <HeaderView />
    <RouterView />
    <BottomButton />
  </div>
</template>

<style scoped></style>
