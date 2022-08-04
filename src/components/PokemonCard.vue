<template>
  <div class="pokemon-card-container" :style="{ background: background }">
    <h3>{{ pokemonName }}</h3>
    <img :src="pokemonImage" alt="pokemon image" class="pokemon-image" />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  props: {
    pokemonName: {
      type: String,
      required: true,
    },
    pokemonImage: {
      type: String,
    },
    pokemonType: {
      type: String,
    },
  },
  setup() {
    return {};
  },
  computed: {
    background() {
      return "#fff";
    },
  },
});
</script>

<style lang="scss" scoped>
.pokemon-card-container {
  height: 300px;
  width: 120px;
}

.pokemon-image {
  max-width: 100%;
}
</style>
