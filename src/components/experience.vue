<template>
 <section class="resume-section" id="experience">
                <div class="resume-section-content">
                    <h2 class="mb-5">Experience</h2>
                    <div class="d-flex flex-column flex-md-row justify-content-between mb-5" v-for="(exp,index) in experiences" :key="index">
                        <div class="flex-grow-1">
                            <h3 class="mb-0">{{exp.title}}</h3>
                            <div class="subheading mb-3">{{exp.company}}</div>
                            <p>{{exp.description}}</p>
                        </div>
                        <div class="flex-shrink-0"><span class="text-primary">March 2013 - Present</span></div>
                    </div>
                </div>
            </section>
</template>

<script>
export default {
  name: 'experience',
  data: function() {
    return {experiences:[
      {
      title:'Senior Web Developer',
      company:'Intelitec Solutions',
      description:'Bring to the table win-win survival strategies to ensure proactive domination. At the end of the day, going forward, a new normal that has evolved from generation X is on the runway heading towards a streamlined cloud solution. User generated content in real-time will have multiple touchpoints for offshoring.'
      },
      {
      title:'Web Developer',
      company:'Intelitec Solutions',
      description:'Capitalize on low hanging fruit to identify a ballpark value added activity to beta test. Override the digital divide with additional clickthroughs from DevOps. Nanotechnology immersion along the information highway will close the loop on focusing solely on the bottom line.'
      },
      {
        title:'Junior Web Designer',
        company:'Shout! Media Productions',
        description:'Podcasting operational change management inside of workflows to establish a framework. Taking seamless key performance indicators offline to maximise the long tail. Keeping your eye on the ball while performing a deep dive on the start-up mentality to derive convergence on cross-platform integration.'
      },
      {
        title:'Web Design Intern',
        company:'Shout! Media Productions',
        description:'Collaboratively administrate empowered markets via plug-and-play networks. Dynamically procrastinate B2C users after installed base benefits. Dramatically visualize customer directed convergence without revolutionary ROI.'
      }
    ]
  }
  }
}
</script>
