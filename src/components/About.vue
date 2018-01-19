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
          I like building useful things and solving wicked problems, that's why I'm a software engineer. The human mind is a puzzle I hope to unravel within my lifetime, but for now I'll use the puzzle pieces to devise intelligent systems. 
          <br /><br />
          My other lifelong pursuits include music and <a target="_blank" rel="noopener" href="https://www.instagram.com/hanyangtay">art</a>. Watch me in twenty years.
          <br /><br />
          <a href="https://docs.google.com/document/d/1b8n4lGHxyCqcvz8ju6Oi5d9HHYIkizBhndt9yToCcaw/edit?usp=sharing"
            rel="noopener" target="_blank">
          <button class="mdc-button mdc-button--raised mdc-ripple-surface">
            <i class="material-icons">description</i>
            Resume
          </button>
          </a>

          <br /><br />
        </div>

    </div>
  </div>

  <div class="mdc-layout-grid content-wrapper" style="padding-top:0em">
    <h2 style="text-align: center"> Irrelevant Experience </h2>
    <div class="mdc-layout-grid__inner">
      <div class="mdc-layout-grid__cell--span-1"></div>
      <div class="mdc-layout-grid__cell--span-3 irrele">
        <img alt="han yang" class="irrele-photo" 
            v-bind:src="irrele1" />
            <br />
        Led a platoon of 6 teams in
        <a href="https://en.wikipedia.org/wiki/Singapore_Combat_Engineers#39th_Battalion,_Singapore_Combat_Engineers_(39SCE)" rel="noopener" target="_blank">
        CBRD</a> operations.
      </div>
      <div class="mdc-layout-grid__cell--span-4 irrele">
        <img alt="han yang" class="irrele-photo" 
            v-bind:src="irrele2" />
            <br />
        Stare at people's brains in
        <a href="http://mindlab.research.wesleyan.edu/" rel="noopener" target="_blank">
        MIND lab</a>.
      </div>
      <div class="mdc-layout-grid__cell--span-3 irrele">
        <img alt="han yang" class="irrele-photo" 
            v-bind:src="irrele3" />
        <br />
        Taught in <a href="http://www.pathlight.org.sg/" rel="noopener" target="_blank">
        Pathlight School (autism)</a> and
        <a href="http://www.wesleyan.edu/cpe/" rel="noopener" target="_blank">
          Center for Prison Education
        </a>
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
      coverPhoto: require('../assets/images/main/about.jpg'),
      irrele1: require('../assets/images/irrelevant/gasmask.png'),
      irrele2: require('../assets/images/irrelevant/researcher.png'),
      irrele3: require('../assets/images/irrelevant/teacher.png')
    }
  },
  mounted () {
    MDCRipple.attachTo(document.querySelector('.mdc-button'))
  }
}
</script>

<style scoped>
.irrele-photo {
  max-width: 100px;
  height: auto;
}

.irrele {
  text-align: center;
}

</style>


