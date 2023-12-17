<script setup lang="ts">
import { RouterLink } from 'vue-router'
// defineProps<{
//   msg: string
// }>()
// TODO: configure prettier, format on save
</script>

<template>
    <!-- <img alt="Vue logo" class="logo" src="@/assets/images/logo.svg" width="65" height="65" /> -->


  <div class="greetings">
    <!-- <h1 class="green">{{ msg }}</h1> -->
    <!-- <h3>
      You’ve successfully created a project with
      <a href="https://vitejs.dev/" target="_blank" rel="noopener">Vite</a> +
      <a href="https://vuejs.org/" target="_blank" rel="noopener">Vue 3</a>. What's next?
    </h3> -->
  </div>

  <nav class="nav">
    <!-- <img class="nav__logo" alt="Vue logo" src="@/assets/logo.png"> -->
    <img alt="Vue logo" class="logo" src="@/assets/images/logo.svg" width="65" height="65" />
    <div class="nav__links">
      <RouterLink class="nav__link link" to="/">Intro</RouterLink>
      <RouterLink class="nav__link link" to="/about">About</RouterLink>
      <RouterLink class="nav__link link" to="/rendering">Rendering</RouterLink>
      <!-- <RouterLink class="nav__link link" to="/components">Components</RouterLink>
      <RouterLink class="nav__sublink link" to="/properties">Properties</RouterLink>
      <RouterLink class="nav__sublink link" to="/hooks">Lifecycle hooks</RouterLink>
      <RouterLink class="nav__link link" to="/slots">Slots</RouterLink>
      <RouterLink class="nav__link link" to="/vue-router">Vue Router</RouterLink>
      <RouterLink class="nav__link link nav__link--glossary" to="/glossary">Glossary</RouterLink>
      <RouterLink class="nav__link link" to="/random">Random</RouterLink> -->
    </div>
  </nav>

</template>

<style scoped lang="scss">
/* h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
} */

/* @media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
} */

.nav {
  grid-area: 1/1/2/2;
  // padding-left: 10px;
  .nav__logo {
    height: 100px;
    width: 100px;
  }
  .nav__links {
    display: flex;
    flex-direction: column;
    align-items: flex-start;

    .nav__link,
    .nav__sublink {
      &.RouterLink-exact-active {
        /* color: $madison; */
        font-weight: bold;
      }
    }

    .nav__sublink {
      margin-left: 10px;
    }

    // .nav__link--glossary {
    //   margin-top: 5px;
    // }

  }
}


</style>
