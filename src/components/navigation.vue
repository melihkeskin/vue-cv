<template>
            <nav class="navbar navbar-expand-lg navbar-dark bg-dark fixed-top" id="sideNav">
            <a class="navbar-brand js-scroll-trigger" href="#page-top">
                <span class="d-block d-lg-none">Clarence Taylor</span>
                <span class="d-none d-lg-block"><img class="img-fluid img-profile rounded-circle mx-auto mb-2" src="@/assets/img/profile.jpg" alt="" /></span>
            </a>
            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation"><span class="navbar-toggler-icon"></span></button>
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav">
                    <li class="nav-item"><a class="nav-link js-scroll-trigger" href="#about">A propos de</a></li>
                    <li class="nav-item"><a class="nav-link js-scroll-trigger" href="#experience">Expérience Professionnelle</a></li>
                    <li class="nav-item"><a class="nav-link js-scroll-trigger" href="#education">Formation</a></li>
                    <li class="nav-item"><a class="nav-link js-scroll-trigger" href="#skills">Compétences</a></li>
                    <li class="nav-item"><a class="nav-link js-scroll-trigger" href="#interests">Intérêts</a></li>
                    <li class="nav-item"><a class="nav-link js-scroll-trigger" href="#interests">Langues</a></li>
                    <li class="nav-item"><a class="nav-link js-scroll-trigger" href="#awards" v-if="false">Cours</a></li>
                </ul>
            </div>
        </nav>
</template>

<script>
export default {
  name: 'navigation',
}
</script>