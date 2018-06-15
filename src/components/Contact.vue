<template>
  <div class="about">
    <navigation></navigation>
    <div class="mdc-layout-grid content-wrapper">
      <div class="mdc-layout-grid__inner">
        
        <div class="mdc-layout-grid__cell--span-1"></div>
        <div class="mdc-layout-grid__cell--span-4">
          <img alt="contact" class="cover-photo" 
          <img alt="han yang" class="cover-photo" 
            v-bind:src="coverPhoto" />
        </div>
        
        <div class="mdc-layout-grid__cell--span-6 text-wrapper">
          <br />
          <br />
          <h2> Contact </h2>
          I'd love to chat! About anything, really. <br /><br />
          
          Feel free to send me an e-mail at <a target="_blank" rel="noopener" href="mailto:htay@wesleyan.edu">htay@wesleyan.edu</a>. 
          <br />You may also find me at any of the social media links below.
          <br /><br />
          Thanks for stopping by, and let me know if there is anything I can do to help.

          <br /><br />
        </div>

      </div>
    </div>
    </div>
  </div>
</template>

<script>
import Navigation from '../components/Navigation.vue'

export default {
  name: 'Contact',
  components: {
    Navigation
  },
  data () {
    return {
      coverPhoto: require('../assets/images/main/contact.jpg')
    }
  }
}
</script>
