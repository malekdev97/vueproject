<script setup>
import { RouterLink, RouterView } from 'vue-router';
</script>

<template>
 
 <nav class="navbar navbar-expand-lg navbar-light bg-light">
  <button class="navbar-toggler navbar-toggler-right" type="button" data-toggle="collapse" data-target="#navbarTogglerDemo02" aria-controls="navbarTogglerDemo02" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>
  <RouterLink to="/" class="navbar-brand ">Vue 3</RouterLink>

  <div class="collapse navbar-collapse" id="navbarTogglerDemo02">
    <ul class="navbar-nav mr-auto mt-2 mt-md-0">
      <li class="nav-item">
        <RouterLink to="/about" class="nav-link ">About</RouterLink>
      </li>
    </ul>
  </div>
</nav>

  <RouterView />
</template>

<style scoped>
.router-link-exact-active {
  color: darkorange;
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
   
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}
 
</style>
