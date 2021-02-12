<template>
  <div class="container">
    <Head />
    <div>
      <Logo />
      <h1 class="title">
        nuxt1
      </h1>
      <div class="links">
        <a
          href="https://nuxtjs.org/"
          target="_blank"
          rel="noopener noreferrer"
          class="button--green"
        >
          Documentation
        </a>
        <a
          href="https://github.com/nuxt/nuxt.js"
          target="_blank"
          rel="noopener noreferrer"
          class="button--grey"
        >
          GitHub
        </a>
      </div>
    </div>
  </div>
</template>

<script>
import Head from '~/components/Head.vue'
export default {
  components:{
    Head
  }
}
</script>

<style>

</style>
