<template lang="html">
  <div class="header">
    <div class="logo wrapper">
      <app-logo color="#fff"></app-logo>
      <p class="logo-title"><strong class="text-bold">Markd</strong>.it</p>
    </div>
    <div class="description wrapper">
      <h1>Open Source Bookmark Manager</h1>
      <p>There will be stuff added to this.</p>
    </div>
    <div class="screenshot">
      <img src="http://via.placeholder.com/860x560" alt="Screenshot of Markd Program">
    </div>
  </div>
</template>

<script>
import Logo from './Logo.vue'

export default {
  components: {
    appLogo: Logo
  }
}
</script>

<style lang="css">

</style>
