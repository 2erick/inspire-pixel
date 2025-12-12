<script setup>
// npm install @iconify/vue
// import { Icon } from "@iconify/vue";
</script>

<template>
  <header>
    <img src="../assets/logo.png" alt="Logo" />

    <nav>
      <ul>
        <li>
          <a href="#">
            Lupa
            <!-- <Icon icon="material-symbols:search" width="24" height="24" /> -->
          </a>
        </li>
        <li><a href="#">Inicio</a></li>
        <li><a href="#">Galeria</a></li>
        <li><a href="#">Favoritos</a></li>
        <li>
          <a href="#"
            ><Icon icon="material-symbols:person" width="24" height="24"
          /></a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<style scoped lang="scss">
header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-wrap: wrap;
  margin: 2rem;

  ul {
    gap: 1.5rem;
    display: flex;
    flex-wrap: wrap;
    list-style: none;
  }

  a {
    text-decoration: none;
    color: black;
  }
}
</style>


<!-- <script setup>
  import { ref } from "vue";
  
  const aberto = ref(false);
  </script>
  
  <template>
    <header>
      <img src="../assets/logo.png" alt="Logo" />
  
      <!-- Botão hambúrguer -->
      <!-- <button @click="aberto = !aberto">☰</button> -->
  
      <!-- Menu simples -->
      <!-- <ul v-if="aberto"> -->
        <!-- <li><a href="#">Lupa</a></li>
        <li><a href="#">Inicio</a></li>
        <li><a href="#">Galeria</a></li>
        <li><a href="#">Favoritos</a></li>
        <li><a href="#">Perfil</a></li> -->
      <!-- </ul> -->
    <!-- </header>
  </template> -->