<template>
  <div class="about">
    <navigation></navigation>
    <div class="mdc-layout-grid content-wrapper">
      <div class="mdc-layout-grid__inner">
        
        <div class="mdc-layout-grid__cell--span-1"></div>
        <div class="mdc-layout-grid__cell--span-4">
          <img alt="han yang" class="cover-photo" 
            v-bind:src="coverPhoto" />
        </div>
        
        <div class="mdc-layout-grid__cell--span-6 text-wrapper">
          <br />
          <br />
          <h2> About Me </h2>
          Psychology/CS Student at Wesleyan University, Class of 2019. 
          <br /><br />
          I like building useful things and solving wicked problems, that's why I'm in this trade of software engineering. The human mind is a puzzle I hope to unravel within my lifetime, but for now I'll use the puzzle pieces to devise intelligent systems. 
          <br /><br />
          My other lifelong pursuits include music and <a target="_blank" rel="noopener" href="https://www.instagram.com/hanyangtay">art</a>. Watch me in twenty years.
          <br /><br />
          <a href="https://docs.google.com/document/d/1b8n4lGHxyCqcvz8ju6Oi5d9HHYIkizBhndt9yToCcaw/edit?usp=sharing"
            rel="noopener" target="_blank">
          <button class="mdc-button mdc-button--raised mdc-ripple-surface">
            <i class="material-icons">description</i>
            Resumé
          </button>
          </a>

          <br /><br />
        </div>

      </div>
    </div>
  </div>
</template>

<script>
import Navigation from '../components/Navigation.vue'
import {MDCRipple} from '@material/ripple'

export default {
  name: 'About',
  components: {
    Navigation
  },
  data () {
    return {
      coverPhoto: require('../assets/images/main/about.jpg')
    }
  },
  mounted () {
    MDCRipple.attachTo(document.querySelector('.mdc-button'))
  }
}
</script>
