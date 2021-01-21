<template>
  <div id="app">
      <!-- Navigation-->
<Navigation/>
        <!-- Page Content-->
        <div class="container-fluid p-0">
            <!-- About-->
         <About/>
            <hr class="m-0" />
            <!-- Experience-->
           <Experience/>
            <hr class="m-0" />
            <!-- Education-->
            <Education/>
            <hr class="m-0" />
            <!-- Skills-->
            <Skill/>
            <hr class="m-0" />
            <!-- Interests-->
             <Interest/>
            <hr class="m-0" />
            <!-- Awards-->
             <Award/>
        </div>
  </div> 
</template>

<script>

import Navigation from './components/navigation'
import About from './components/about'
import Experience from './components/experience'
import Education from './components/education'
import Skill from './components/skill'
import Interest from './components/interest'
import Award from './components/award'

export default {
  name: 'App',
  components:{
      Navigation,
      About,
      Experience,
      Education,
      Skill,
      Interest,
      Award
  }
}
</script>

