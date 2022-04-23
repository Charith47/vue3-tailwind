<template>
  <div>
    <nav>
      <router-link class="pr-2 text-sky-600 underline" to="/">Home</router-link>
      <router-link class="text-sky-600 underline" to="/about">About</router-link>
    </nav>
    <h1 class="text-3xl font-bold">
      Hello from App!
    </h1>
    <router-view>
    </router-view>
  </div>
</template>

<script setup>
</script>


<style>
</style>
