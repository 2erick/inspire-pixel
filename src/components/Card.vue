<script setup>
import { ref } from "vue";

const props = defineProps(["image"]);

// começa como "não curtido"
const liked = ref(false);
</script>

<template>
  <div class="card">
    <!-- Ícone simples -->
    <span @click="liked = !liked">
      {{ liked ? "❤️" : "🤍" }}
    </span>

    <img :src="image" alt="Imagem do card" />
  </div>
</template>

<style scoped lang="scss">
.card {
  position: relative;
  width: 35vw;
  max-width: 350px;
  height: 65vh;
  /* border: solid; */
  border-radius: 10px;
  margin: 10px 0;

  img {
    width: 100%;
    height: 100%;
    border-radius: 10px;
  }

  .icon {
    position: absolute;
    top: 10px;
    right: 10px;
    color: red;
  }
}
</style>
