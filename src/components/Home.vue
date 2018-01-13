<template>
  <div class="home">
    <div class="mdc-layout-grid content-wrapper">
      <div class="mdc-layout-grid__inner">
        
        <div class="mdc-layout-grid__cell--span-1"></div>
        <div class="mdc-layout-grid__cell--span-4">
          <img alt="han yang" class="cover-photo" v-bind:src="coverPhoto" />
        </div>
        
        <div class="mdc-layout-grid__cell--span-6 text-wrapper">
          <br /><br /><br />
          <h1> hi, I'm Han. </h1>
          &nbsp;{{ msg }}
          <br /><br /><br /><br />

          <router-link to="/about">
          <button class="mdc-button mdc-button--raised mdc-ripple-surface"
              id="button-about">
            <i class="material-icons">face</i>
            About
          </button>
          </router-link>

          &nbsp; &nbsp;

          <router-link to="/projects">
          <button class="mdc-button mdc-button--raised mdc-ripple-surface"
            id="button-projects">
              <i class="material-icons">code</i>
            Projects
          </button>
          </router-link>

          &nbsp; &nbsp;
          
          <router-link to="/contact">
          <button class="mdc-button mdc-button--raised mdc-ripple-surface"
            id="button-contact">
              <i class="material-icons">email</i>
            Contact
          </button>
          </router-link>
          <br /><br />
        </div>

      </div>
    </div>
  </div>
</template>

<script>
import {MDCRipple} from '@material/ripple'
export default {
  name: 'Home',
  data () {
    return {
      msg: 'I am a software engineer. I code, I build useful things.',
      coverPhoto: require('../assets/images/main/hy.jpg')
    }
  },
  mounted () {
    MDCRipple.attachTo(document.querySelector('#button-about'))
    MDCRipple.attachTo(document.querySelector('#button-projects'))
    MDCRipple.attachTo(document.querySelector('#button-contact'))
  }
}


</script>

<style scoped>
h1 {
  line-height: 1em;
}
</style>
