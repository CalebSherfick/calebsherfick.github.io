<template>
  <div class="container-fluid">

    <nav
      :class="$mq | mq({xs: 'navbar navbar-expand-lg navi row', sm: 'navbar navbar-expand-lg navi row', md: 'navbar sticky-top navbar-expand-lg navi row', lg: 'navbar sticky-top navbar-expand-lg navi row'})">
      <div class="col-12">
        <div class="row">


          <a :class="$mq | mq({xs: 'navbar-brand nav-text col-12', sm: 'navbar-brand nav-text col-12', md: 'navbar-brand nav-text col-2', lg: 'navbar-brand nav-text col-2'})"
            href="#">Caleb Sherfick</a>


          <a :class="$mq | mq({xs: 'nav-item nav-link active nav-text col-6', sm: 'nav-item nav-link active nav-text col-6', md: 'nav-item nav-link active nav-text offset-5 col-1', lg: 'nav-item nav-link active nav-text offset-5 col-1'})"
            href="#">About
            Me</a>
          <a :class="$mq | mq({xs: 'nav-item nav-link active nav-text col-6', sm: 'nav-item nav-link active nav-text col-6', md: 'nav-item nav-link active nav-text col-1', lg: 'nav-item nav-link active nav-text col-1'})"
            href="#skills">Skills</a>

          <a :class="$mq | mq({xs: 'nav-item nav-link active nav-text col-6', sm: 'nav-item nav-link active nav-text col-6', md: 'nav-item nav-link active nav-text col-1', lg: 'nav-item nav-link active nav-text col-1'})"
            href="#">Portfolio</a>
          <a :class="$mq | mq({xs: 'nav-item nav-link active nav-text col-6', sm: 'nav-item nav-link active nav-text col-6', md: 'nav-item nav-link active nav-text col-1', lg: 'nav-item nav-link active nav-text col-1'})"
            href="#">Contact</a>
        </div>
      </div>
    </nav>

    <header
      :class="$mq | mq({xs: 'jumbotron head-photo-mobile row', sm: 'jumbotron head-photo-mobile row', md: 'jumbotron head-photo row', lg: 'jumbotron head-photo row'})">
      <div class="col-12">
        <div class="row justify-content-start">
          <h1 :class="$mq | mq({xs: 'col', sm: 'col', md: 'col', lg: 'col-4 d-flex justify-content-start'})">Caleb
            Sherfick</h1>
        </div>
        <div class="row justify-content-start">
          <p :class="$mq | mq({xs: 'col', sm: 'col', md: 'col', lg: 'col-4 d-flex justify-content-start'})">Full Stack
            Software Developer</p>
        </div>
        <div class="row justify-content-start">
          <div :class="$mq | mq({xs: 'col', sm: 'col', md: 'col-4', lg: 'col-3 d-flex justify-content-start'})">
            <a class="btn btn-lg btn-color btn-text shadow" href="#" role="button">View Work</a>
          </div>
        </div>
      </div>
    </header>




    <!-- :class="$mq | mq({xs: '', sm: '', md: '', lg: ''})" -->


  </div>
</template>

<script>
  export default {
    name: 'home',
    components: {
    }
  }
</script>

<style>
  .navi {
    background-color: #343534;
  }

  .nav-text {
    color: #f4fffd;
  }

  .nav-text:hover {
    color: white;
    text-shadow: 0px 0px 2px white;
  }

  .nav-text:active {
    color: rgb(187, 187, 187);
    text-shadow: 0px 0px 0px black;
  }

  .head-photo {
    background-image: url("../assets/federica-galli-449563-unsplash.jpg");
    background-size: 100%;
    /* width: 100%; */
    background-position: center 95%;
    background-repeat: no-repeat;
    padding: 20vh;
    border-radius: 0px;
  }

  .head-photo-mobile {
    background-image: url("../assets/federica-galli-449563-unsplash.jpg");
    background-size: 200%;
    /* width: 100%; */
    height: 50vh;
    background-position: center 95%;
    background-repeat: no-repeat;
    border-radius: 0px;
  }

  /* .photo-letters {  
  text-shadow: -1px 1px 2px;
} */

  .btn-color {
    background-color: #67747b;
  }

  .btn-text {
    color: #f4fffd;
  }

  .about-color {
    background-color: #67747b;
    color: #f4fffd;
  }

  .skills-bg {
    background-color: #dde0dc;
    color: #343534;
  }

  .skill-img {
    max-width: 20vh;
  }

  .xp-background {
    background-color: #f4fffd;
    color: #475841
  }

  .foot-color {
    background-color: #2d3142;
    color: #f4fffd;
  }

  .project-text {
    color: #f4fffd;
    text-shadow: -1px 1px 2px;
  }
</style>