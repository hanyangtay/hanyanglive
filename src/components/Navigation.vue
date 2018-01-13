<template>
  <header class="navigation">
    <div class="navigation-container">
    <router-link to="/">
      <img alt="han yang" class="header-home" 
          v-bind:src="homeIcon"/>
    
      <span class="mdc-toolbar__title">hanyang.
        <span class="header-right">live</span>
      </span>
    </router-link>

    <div class="right">

      <router-link to="/about">
        About
      </router-link>

      <router-link to="/projects">
        Projects
      </router-link>

      <router-link to="/contact">
        Contact
      </router-link>

    </div>
    </div>
  </header>
</template>

<script>
import SlidingHeader from '../assets/scripts/slidingHeader'

export default {
  name: 'Navigation',
  data () {
    return {
      homeIcon: require('../assets/images/main/hy.jpg')
    }
  },
  mounted () {
    new SlidingHeader({
      element: 'div.navigation-container',
      class: 'scrolled'
    })
  }
}
</script>

<style scoped>
/* Header */

.navigation-container{
  position: fixed;
  left: 0;
  right: 0;
  background-color: #fff;
<<<<<<< cd4a8617f85d3214757e820366c07b72b2d432b5
  min-height: 6em;
=======
  height: 6em;
>>>>>>> 1.0
  transition: all .4s;
  padding-top: 1em;
  margin-left: auto;
  margin-right: auto;
  width: 100%;
  max-width: 1200px;
  z-index: 20;
}

a {
  transition: opacity 200ms;
}

a:hover {
  opacity: 0.7;
}

.right {
  float: right;
  margin-right: 2em;
}

<<<<<<< cd4a8617f85d3214757e820366c07b72b2d432b5
@media screen and (max-width: 588px) {
  .right{
    float: left;
  }
}

=======
>>>>>>> 1.0
.scrolled {
  transform: translateY(-6em);
}

.header-home {
  width: 72px;
  height: auto;
  margin-left: 2em;
}

.mdc-toolbar__title {
  color: var(--mdc-theme-text-primary-on-primary);
  vertical-align: 1.3em;
}

.header-right {
  color: var(--header-colour);
  margin-left: -5px;
}

.right {
  padding-top: 16px;
  height: 72px;
}

.right a {
  color: #616161;
  display: inline-block;
  height: 3em;
  line-height: 3em;
  font-weight: 300;
  margin-left: 3em;
  border-bottom: 3px solid transparent;
  transition-timing-function: ease-in-out;
  transition: border-bottom 200ms;
}

.right a:hover {
  border-bottom: 3px solid #8bc34a;
}

</style>
