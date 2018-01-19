<template>
  <div id="app">
  <router-view/>



  <footer>
    <a target="_blank" rel="noopener" href="https://github.com/hanyangtay/messenger">
       <img id="footer_github" src="./assets/images/footer/github.png" alt="Github" />
    </a>

    &nbsp;

    <a id="footer_email" href="mailto:htay@wesleyan.edu">
       <i class="material-icons">email</i>
    </a>

    &nbsp;

    <a target="_blank" rel="noopener" href="https://www.linkedin.com/in/hanyang-tay">
       <img id="footer_linkedin" src="./assets/images/footer/linkedin.png" alt="Linkedin" />
    </a>

    <br />
    ©2018 han yang tay
  </footer>



  </div>

  
</template>

<script>
export default {
  name: 'app'
}
</script>

<style>

/* Body text */
:root {
  --header-colour: #7cb342;
  --h1-colour: #8bc34a;
  --link-colour: #d81b60;
  --mdc-theme-primary: #fafafa;
  --mdc-theme-text-primary-on-primary: #383838;
}

/* Layout */
.content-wrapper{
  width:100%;
  padding-top: 6.5em;
}

@media screen and (max-width: 588px) {
  .content-wrapper{
    padding-top: 11.5em;
  }
}

.text-wrapper{
  padding-left: 2.5em;
  padding-right: 2em;
}

body {
  color: var(--mdc-theme-text-primary-on-primary);
  line-height:1.5em;
  margin-top: 0px;
}

h1 {
  color: var(--h1-colour);
  font-size: 72px;
  font-family: Quicksand;
  margin-bottom: 38px;
}

h2 {
  color: var(--h1-colour);
  font-size: 48px;
  font-family: Quicksand;
  margin-bottom: 32px;
}

a {
  text-decoration: none;
  transition-timing-function: ease-in-out;
  transition: color 200ms;
  color: var(--link-colour);
}

a:hover{
  color: var(--header-colour);
}

.cover-photo {
  max-width: 100%;
  height: auto;
}

/* Button style */

.mdc-button {
  margin-bottom: 16px;
}
.mdc-button .material-icons {
  vertical-align: -7px;
  padding-right: 8px;
}


/* Footer */

footer {
  margin: 0em 0  3em 0;
  text-align: center;
  font-size: 16px;
  font-family: Gloria Hallelujah;
  line-height: 2.0em;
}

footer a {
  text-decoration: none;
  opacity: 0.54;
  transition-timing-function: ease-in-out;
  transition: opacity 200ms;
}

footer img {
  -webkit-backface-visibility: hidden;
}

footer a:hover {
  opacity: 1.0;
}

#footer_github {
  height: 1.2em;
  width: 1.2em;
}

#footer_email {
  color: #000;
  size: 24px;
  vertical-align: -2px;
}

#footer_linkedin {
  height: 1.2em;
  width: 1.2em;
}
</style>
