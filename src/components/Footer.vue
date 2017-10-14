<template lang="html">
  <div class="footer">
    <div class="ending wrapper">
      <h2>Community powered</h2>
      <p>Markd is a open source bookmark manager, made with ♥️ by <a href="https://github.com/orgs/markd/people"
                                                                     target="_blank">devcord users</a>.</p>
      <p>To view the <a href="https://github.com/markd/markd" target="_blank">GitHub</a>!</p>
    </div>
    <div class="logo-end">
      <app-logo color="#fff"></app-logo>
    </div>
  </div>
</template>

<script>
import Logo from './Logo.vue'

export default {
  name: 'Footer',
  components: {
    appLogo: Logo
  }
}
</script>

<style lang="css">

</style>
