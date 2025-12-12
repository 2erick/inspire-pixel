<script setup>
import axios from "axios";
import { ref } from "vue";
import Card from "./Card.vue";

const imagens = ref([]);

async function carregarImagens() {
  const res = await axios.get("https://picsum.photos/v2/list?page=3&limit=30");
  imagens.value = res.data;

  console.log(res)
}
carregarImagens();
</script>

<template>
  <h2>Inspire-se</h2>
  <section class="inspirese">
    <Card v-for="img in imagens" :key="img.id" :image="img.download_url" />
  </section>
</template>

<style scoped lang="scss">
.inspirese,
h2 {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  margin: 2rem;
}
</style>
