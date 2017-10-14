<template>
  <div id="app">
    <app-header></app-header>
    <app-content></app-content>
    <app-footer></app-footer>
    <router-view/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Content from './components/Content.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'app',
  components: {
    appHeader: Header,
    appContent: Content,
    appFooter: Footer
  }
}
</script>

<style>

/* DEBUGGING */
!
* {
  box-sizing: border-box;
  border-style: dotted;
  border-width: 1px;
  ! border-color: white;
}

/* MOBILE */
html {
  text-size-adjust: 100%;
  font-family: Open Sans, sans-serif;
}

body {
  font-size: 14px;
  letter-spacing: 1px;
  margin: 0;
}

:root {
  --main-color: #fe813a;
  --space: 75px;
  --width: 560px;
}

.wrapper {
  width: 90%;
  max-width: 1060px;
  margin: 0 auto;
  overflow: hidden;
}

.flexbox {
  display: flex;
  align-items: center;
  justify-content: center;
}

/* Header */
.header {
  background: var(--main-color);
  background: radial-gradient(var(--main-color), #c76127);
}

.logo {
  padding: var(--space) 0px var(--space) 0px;
}

.logo-title {
  color: white;
  font-family: Open Sans;
  text-transform: uppercase;
  font-size: 30px;
  letter-spacing: 2.5px;
  margin: 0;
  text-align: center;
}

.text-bold {
  font-weight: 900;
}

svg {
  height: 150px;
  display: block;
  margin: 0 auto;
}

/* Description */
.description {
  max-width: var(--width);
}

.description h1, .description p {
  color: white;
  text-align: center;
}

.description h1 {
  font-size: 30px;
  margin: 0px;
}

.description p {
  font-size: 16px;
  margin-bottom: var(--space);
}

/* Screenshot */
.screenshot img {
  display: block;
  margin: auto;
  width: var(--width);
  margin-bottom: var(--space);
}

.screenshot {
  overflow: hidden;
}

/* Content */
.content h2 {
  text-align: center;
}

.content a {
  color: var(--main-color);
  text-decoration: none;
  text-transform: uppercase;
  font-weight: bold;
  font-size: 18px;
}

.design {
  position: relative;
  overflow: visible;
  text-align: left;
  max-width: var(--width);
  border: 1px solid #dbdbdb;
  border-radius: 5px;
  margin-bottom: 30px;

}

.design img {
  display: block;
  margin: auto;
}

.circle {
  position: absolute;
  top: 30px;
  left: -25px;
  height: 40px;
  width: 40px;
  border-radius: 50%;
  text-align: center;
  font-size: 28px;
  font-weight: bolder;
  color: white;
  background-color: var(--main-color);
}

/* Footer */
.footer {
  background: var(--main-color);
  background: radial-gradient(var(--main-color), #c76127);
  color: white;
  padding: var(--space) 0px var(--space) 0px;
}

.footer a {
  color: white;
  font-weight: bolder;
}

.ending {
  max-width: var(--width);
  text-align: left;
}

.logo-end svg {
  margin-top: var(--space);
  height: 50px;
}

</style>
