<template>
  <div class="container">
    <h1>Pokedex</h1>
    <Paginator :page="1" />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import Paginator from "../components/Paginator.vue";

export default defineComponent({
  setup() {
    return {};
  },
  components: { Paginator },
});
</script>

<style scoped></style>
