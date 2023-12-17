<script setup lang="ts">
import { RouterView } from 'vue-router'
import ContentList from './components/ContentList.vue'
</script>

<template>
  <header>

  </header>
  <aside>
    <div class="wrappr" style="border: 1px solid red">
      <ContentList />
    </div>    
  </aside>
  <main style="border: 1px solid red">
    <RouterView />
  </main>
  <footer>

  </footer>

</template>

<style src="./assets/styles/app.scss" scoped lang="scss" />
