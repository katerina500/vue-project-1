<script>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <a-layout>
      <a-layout-sider>Sider</a-layout-sider>
      <a-layout>
      <a-layout-header>
        <a-button type="primary" href="/">Home</a-button>
        <a-button type="primary" href="/about">About</a-button>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </a-layout-header>
        <a-layout-content><RouterView /></a-layout-content>
        <a-layout-footer>Footer</a-layout-footer>
      </a-layout>
    </a-layout>
    <template>
  <a-menu v-model:selectedKeys="current" mode="horizontal" :items="items" />
</template>



</template>



