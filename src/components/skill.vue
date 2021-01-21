<template>
    <section class="resume-section" id="skills">
                <div class="resume-section-content">
                    <h2 class="mb-5">Skills</h2>
                    <div class="subheading mb-3">Programming Languages & Tools</div>
                    <ul class="list-inline dev-icons">
                        <li class="list-inline-item" v-for="(wr, index) in skills" :key="index"><i v-bind:class="wr.class"></i></li>
                    </ul>
                    <div class="subheading mb-3">Workflow</div>
                    <ul class="fa-ul mb-0">
                        <li  v-for="(wr, index) in workFlows" :key="index">
                            <span class="fa-li"><i class="fas fa-check"></i></span>
                            {{wr.work}}
                        </li>
                    </ul>
                </div>
            </section>
</template>

<script>
export default {
  name: 'skill',
  data:function(){
      return {
          skills:[
              { name:'html5',  class:'fab fa-html5' },
              { name:'css3',  class:'fab fa-css3-alt' },
              { name:'js',  class:'fab fa-js-square' },
              { name:'angular',  class:'fab fa-angular' },
              { name:'react',  class:'fab fa-react' },
              { name:'nodejs',  class:'fab fa-node-js' },
              { name:'sass',  class:'fab fa-sass' },
              { name:'less',  class:'fab fa-less' },
              { name:'wordpress',  class:'fab fa-wordpress' },
              { name:'gulp',  class:'fab fa-gulp' },
              { name:'grunt',  class:'fab fa-grunt' },
              { name:'npm',  class:'fab fa-npm' },
              ],
          workFlows:[
              { work:'Mobile-First, Responsive Design'},
              { work:'Cross Browser Testing & Debugging'},
              { work:'Cross Functional Teams'},
              { work:'Agile Development & Scrum'},
              ]
      }
  }
}
</script>