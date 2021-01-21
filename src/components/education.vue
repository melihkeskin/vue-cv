<template>
    <section class="resume-section" id="education">
                <div class="resume-section-content">
                    <h2 class="mb-5">Education</h2>
                    <div class="d-flex flex-column flex-md-row justify-content-between mb-5" v-for="(edu, index) in educations" :key="index">
                        <div class="flex-grow-1">
                            <h3 class="mb-0">{{edu.school}}</h3>
                            <div class="subheading mb-3">{{edu.faculty}}</div>
                            <div v-if="edu.major">{{edu.major}}</div>
                            <p>GPA: {{edu.gpa}}</p>
                        </div>
                        <div class="flex-shrink-0"><span class="text-primary">{{edu.startDate}} - {{edu.endDate}}</span></div>
                    </div>
                </div>
            </section>
</template>

<script>
export default {
  name: 'education',
  data:function(){
      return {
          educations:[
              {
                  school:'University of Colorado Boulder',
                  faculty:'Bachelor of Science',
                  major:'Computer Science - Web Development Track',
                  startDate:'August 2006',
                  endDate:'May 2010',
                  gpa: '3.56'
              },
              {
                  school:'James Buchanan High School',
                  faculty:'Technology Magnet Program',
                  major:'',
                  startDate:'August 2002',
                  endDate:'May 2006',
                  gpa: '3.23'
              }
              ]
      };
  }
}
</script>