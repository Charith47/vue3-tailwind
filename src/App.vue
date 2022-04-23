<template>
  <div>
    <h1 class="text-3xl font-bold">
      Hello from App!
    </h1>
    <nav>
      <router-link class="pr-2 text-sky-600 underline" to="/">Home</router-link>
      <router-link class="text-sky-600 underline" to="/about">About</router-link>
    </nav>
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  setup() {
    const data = 'Hello from setup!'
    return {
      data
    }
  },
  mounted() {
    console.log(this.data)
  }
}
</script>
