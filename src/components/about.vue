<template>
    <section class="resume-section" id="about">
                <div class="resume-section-content">
                    <h1 class="mb-0">
                        {{personal.name}}
                        <span class="text-primary">{{personal.surname}}</span>
                    </h1>
                    <div class="subheading mb-5">
                        {{personal.address}} ·
                        <a href="mailto:name@email.com">{{personal.email}}</a>
                    </div>
                    <p class="lead mb-5">
                      J’ai 10 ans d'expériences professionnelle. J’ai travaillé sur un certain nombre de projets comme la gestion de la relation client, intégration bancaire, services de backend pour l'application mobile, projet web, intégration d'applications avec cloud et en plus j'ai un certificat MCPD.
                      </p>
                    <div class="social-icons">
                        <a class="social-icon" target="_blank" v-for="(sc,index) in personal.socials" :key="index" v-bind:href="sc.address"><i v-bind:class="sc.class"></i></a>
                    </div>
                </div>
            </section>
</template>

<script>
export default {
  name: 'about',
  data: function () {
    return {
        personal: {
          name:'Melih',
          surname:'Keskin',
          address:'45000 Orléans, France· (+33) 07.49.14.56.93',
          email:'melihkeskinn@gmail.com',
          description:"J’ai 10 ans d'expériences professionnelle. J’ai travaillé sur un certain nombre de projets comme la gestion de la relation client, intégration bancaire, services de backend pour l'application mobile, projet web, intégration d'applications avec cloud et en plus j'ai un certificat MCPD.",
          socials:[
            {
            class:'fab fa-linkedin-in',
            address:'linkedin'
          },
          {
            class:'fab fa-github',
            address:'github'
          }
          ]
        }
    };
  }
}
</script>
