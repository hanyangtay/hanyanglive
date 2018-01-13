<template>
  <div class="projects">
    <navigation></navigation>
    <div class="mdc-layout-grid content-wrapper">
      <div class="mdc-layout-grid__inner">
        
        <div class="mdc-layout-grid__cell--span-1"></div>
        <div class="mdc-layout-grid__cell--span-4">
          <img alt="projects" class="cover-photo" 
            v-bind:src="coverPhoto" />
        </div>
        
        <div class="mdc-layout-grid__cell--span-6 text-wrapper">
          <h2> Projects </h2>
          Play with the demos!
          <br /><br />
          <div class="ih-item circle">
            <a href="#computer-vision">
            <div class="spinner"></div>
            <div class="img">
              <i class="material-icons project_icon">remove_red_eye</i>
            </div>
            <div class="info two-lines">
            <div class="info-back">
              <h3>Computer Vision</h3>
            </div>
            </div>
            </a>
          </div>
              
          <div class="ih-item circle">
            <a href="#twitter">
              <div class="spinner"></div>
              <div class="img">
                <i class="material-icons project_icon">format_quote</i>
              </div>
              <div class="info">
              <div class="info-back">
                <h3>Twitter</h3>
              </div>
              </div>
            </a>
          </div>


              
              <div class="ih-item circle">
                <a href="#messenger">
                  <div class="spinner"></div>
                  <div class="img">
                    <i class="material-icons project_icon">chat_bubble_outline</i>
                  </div>
                  <div class="info">
                  <div class="info-back">
                    <h3>Messenger</h3>
                  </div>
                  </div>
                </a>
              </div>

              <div class="ih-item circle">
                <a href="#maps">
                  <div class="spinner"></div>
                  <div class="img">
                    <i class="material-icons project_icon">local_taxi</i>
                  </div>
                  <div class="info">
                  <div class="info-back">
                    <h3>Maps</h3>
                  </div>
                  </div>
                </a>
              </div>





      </div>
    </div>

    <!-- start of project blurbs -->
    <div class="mdc-layout-grid__inner">
        <div class="mdc-layout-grid__cell--span-2"></div>
        <div class="mdc-layout-grid__cell--span-8">

            <div class="projects-block" id="computer-vision">  
              <a href="https://github.com/hanyangtay/neural-networks" class="project-title" target="_blank" rel="noopener">
              Computer Vision
              </a>

              <span class="project-links">
              <a href="https://github.com/hanyangtay/neural-networks" class ="demo" target="_blank" rel="noopener">
                DEMO
              </a>
              &nbsp; &nbsp;
              <a href="https://github.com/hanyangtay/neural-networks" target="_blank" rel="noopener">
              <img v-bind:src="github" class="projects-github-icon" />
              </a>
              </span>
              <hr>
              <h4> Concept: </h4>
              Trained several convolutional neural networks to classifiy images from the CIFAR-10 dataset.
              <br /><br />
              <a href="https://github.com/hanyangtay/neural-networks" target="_blank" rel="noopener">
              <img v-bind:src="cnn" class="projects-images">
              </a>
              <h4>Features: </h4>
              <ul>
                <li> Best performance over 1000 test images: 84.6%</li>
                <li> Activation units: Affine Transformation, ReLU, Convolutional layers </li>
                <li> Learning algorithms: Stochastic Gradient Descent, Momentum, RMSProp , Adam, Momentum  </li>
                <li> Optimisations: Pooling layers, Batch Normalisation, Dropout, L2 Regularisation</li>
                <li> Other classifiers: Support Vector Machine, k-Nearest Neighbours, Softmax, Fully Connected Nets </li>
              </ul>
              
              <h4>Tools used:</h4>
               Python, numPy, Jupyter notebook, Cython
              

            </div>
        
            <div class="projects-block" id="twitter">  
              <a href="https://twitter-hanyang.herokuapp.com" class="project-title" target="_blank" rel="noopener">
              Twitter
              </a>

              <span class="project-links">
              <a href="https://twitter-hanyang.herokuapp.com" class ="demo" target="_blank" rel="noopener">
                DEMO
              </a>
              &nbsp; &nbsp;
              <a href="https://github.com/hanyangtay/twitter" target="_blank" rel="noopener">
              <img v-bind:src="github" class="projects-github-icon" />
              </a>
              </span>
              <hr>
              <h4> Concept: </h4>
              I copied Twitter with Ruby on Rails to learn web development.
              <br /><br />
              <a href="https://hanyangtay.herokuapp.com/login" target="_blank" rel="noopener">
              <img v-bind:src="twitter" class="projects-images">
              </a>
              <h4>Features: </h4>
              <ul>
                <li> User authentication </li>
                <li> Follow, like, retweet </li>
                <li> Picture uploads with live preview</li>
                <li> E-mails for sign-ups and password resets </li>
              </ul>
              
              <h4>Tools used:</h4>
               Ruby on Rails, jQuery, PostgreSQL
              

            </div>

            <div class="projects-block" id="messenger">  
              <a href="https://messenger.hanyang.live" class="project-title" target="_blank" rel="noopener">
              Messenger
              </a>

              <span class="project-links">
              <a href="https://messenger.hanyang.live" class ="demo" target="_blank" rel="noopener">
                DEMO
              </a>
              &nbsp; &nbsp;
              <a href="https://github.com/hanyangtay/messenger" target="_blank" rel="noopener">
              <img v-bind:src="github" class="projects-github-icon" />
              </a>
              </span>
              <hr>
              <h4> Concept: </h4>

              Simple live chat app. Leave a message in the depths of the internet. Say hi.
              <br /><br />
              <a href="https://hanyangtay.herokuapp.com/live_chat" target="_blank" rel="noopener">
              <img v-bind:src="messenger" class="projects-images">
              </a>
              <h4>Features: </h4>
              <ul>
                
                <li> Live. Try using two accounts and talk to yourself. </li>
                <li> View users who are currently online. </li>
              </ul>
              
              <h4>Tools used:</h4>
               Go, VueJS, WebSocket, PostgreSQL

            </div>


            <div class="projects-block" id="maps">  
              <a href="https://github.com/hanyangtay/asteria" class="project-title" target="_blank" rel="noopener">
              Maps
              </a>

              <span class="project-links">
              <a href="https://github.com/hanyangtay/asteria" class ="demo" target="_blank" rel="noopener">
                DEMO
              </a>
              &nbsp; &nbsp;
              <a href="https://github.com/hanyangtay/asteria" target="_blank" rel="noopener">
              <img v-bind:src="github" class="projects-github-icon" />
              </a>
              </span>
              <hr>
              <h4> Concept: </h4>
              Map service that routes between two locations with a <a href="https://en.wikipedia.org/wiki/Map_matching" target="_blank" rel="noopener">map-matching</a> module that I developed for
              <a href="https://swatmobile.io" target="_blank" rel="noopener">SWAT</a>, a taxi ridesharing startup, over summer 2017.

              <br /><br />

              <a href="https://swatmobile.io" target="_blank" rel="noopener">
              <img v-bind:src="maps" class="projects-images">
              </a>

              <h4>Features: </h4>
              <ul>
                
                <li> Uses an edge-expanded graph representation and implements the following routing algorithms: Dijkstra, A* Search, Contraction Hierarchies and their bidirectional variants </li>
                <li> ETA varies by the hour and takes into account morning and evening traffic rush hours </li>
                <li> Implemented <a href="https://www.microsoft.com/en-us/research/publication/hidden-markov-map-matching-noise-sparseness/" target="_blank" rel="noopener">Newson & Krumm's algorithm</a> based on time inhomogeneous Hidden Markov Model processes from scratch in Go </li>
                <li> Spatial and temporal accuracy of matched results exceed performance of map-matching algorithms implemented by existing open source software such as <a href="https://www.graphhopper.com/" target="_blank" rel="noopener">Graphhopper</a> and <a href="http://project-osrm.org/" target="_blank" rel="noopener">OSRM</a> </li>
              </ul>
              
              <h4>Tools used:</h4>
               Go, OpenStreetMap, Leaflet              

            </div>






          </div>

        </div>
    </div>
  </div>
  </div>
</template>

<script>
import Navigation from '../components/Navigation.vue'

export default {
  name: 'Projects',
  components: {
    Navigation
  },
  data () {
    return {
      coverPhoto: require('../assets/images/main/projects.jpg'),
      github: require('../assets/images/footer/github.png'),
      maps: require('../assets/images/showcase/maps.jpg'),
      cnn: require('../assets/images/showcase/cnn.jpg'),
      twitter: require('../assets/images/showcase/twitter.jpg'),
      messenger: require('../assets/images/showcase/messenger.jpg')
    }
  }
  
}
</script>

<style scoped>

.projects-block {
  margin-top: 4em;
  padding-top: 3em;
}

.projects-block, ul{
    font-size: 18px;
    line-height: 32px;
    font-weight: 300;
}

.projects-images{
    height: 50%;
    width: 50%;
    border: 1px solid #e1e8ed;
    border-radius: 6px;
    
  }

.project-links {
  float:right;
}

.demo {
  font-size: 16px;
  font-weight: 800;
}

 .projects-github-icon {
    margin-right: 0.5em;
    height: 18px;
    width: 18px;
    opacity: 0.7;
    -webkit-backface-visibility: hidden;
 }

/* Titles */
.project-title {
  color: #424242;
  font-size: 48px;
  font-weight: 500;
}

.project-title:hover {
  color: var(--header-colour);
}

h4 {
  font-size: 28px;
  color: #737373; 
  margin-bottom: 10px;
}

.projects-block a img {
  opacity: 0.7;
  transition: opacity 200ms ease-in-out;
}
.projects-block a img:hover{
  opacity: 1.0;
}

/* iHover from http://gudh.github.io/ihover/dist/ */

.ih-item {
  float:left;
  position: relative;
  margin-right: 2em;
  margin-bottom: 2em;
  -webkit-transition: all 0.35s ease-in-out;
  -moz-transition: all 0.35s ease-in-out;
  transition: all 0.35s ease-in-out;
  cursor: pointer;
}

.ih-item,
.ih-item * {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}

.ih-item a {
  color: #333;
}

.ih-item.circle {
  width: 10em;
  height: 10em;
  border-radius: 50%;
}

.material-icons.project_icon {
  font-size:36px;
  -ms-transform: translate(62px, -102px);
  /* IE 9 */
  -webkit-transform: translate(62px, -102px);
  /* Safari */
  transform: translate(62px, -102px);
}

.ih-item.circle .info {
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  text-align: center;
  border-radius: 50%;
  -webkit-backface-visibility: hidden;
  backface-visibility: hidden;
}

.ih-item.circle .spinner {
  width: 10em;
  height: 10em;
  border: 0.6em solid #757575;
  border-right-color: #1ad280;
  border-bottom-color: #1ad280;
  border-radius: 50%;
  -webkit-transition: all 0.8s ease-in-out;
  -moz-transition: all 0.8s ease-in-out;
  transition: all 0.8s ease-in-out;
}


.ih-item.circle .info {
  top: 0px;
  left: 0px;
  background: #333333;
  background: rgba(0, 0, 0, 0.6);
  opacity: 0;
  -webkit-transition: all 0.8s ease-in-out;
  -moz-transition: all 0.8s ease-in-out;
  transition: all 0.8s ease-in-out;
}

.ih-item.circle .info h3 {
  color: #fff;
  text-transform: uppercase;
  position: relative;
  letter-spacing: 2px;
  line-height: 30px;
  font-size: 18px;
  margin: 0px 10px;
  padding-top: 60px;
  height: 100px;
  text-shadow: 0 0 1px white, 0 1px 2px rgba(0, 0, 0, 0.3);
}

.ih-item.circle .info.two-lines h3{
  padding-top: 45px;
}

.ih-item.circle a:hover .spinner {
  -webkit-transform: rotate(180deg);
  -moz-transform: rotate(180deg);
  -ms-transform: rotate(180deg);
  -o-transform: rotate(180deg);
  transform: rotate(180deg);
}

.ih-item.circle a:hover .info {
  opacity: 1;
}


</style>
