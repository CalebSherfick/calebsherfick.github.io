<template>
  <div class="container-fluid">

    <nav class="navbar sticky-top navbar-expand-lg navi">
      <a class="navbar-brand nav-text" href="#">Caleb Sherfick</a>
      <div class="navbar-nav">
        <a class="nav-item nav-link active nav-text" href="#">About Me</a>
        <a class="nav-item nav-link active nav-text" href="#skills">Skills</a>
        <a class="nav-item nav-link active nav-text" href="#">Experience</a>
        <a class="nav-item nav-link active nav-text" href="#">Portfolio</a>
        <a class="nav-item nav-link active nav-text" href="#">Contact</a>
      </div>
    </nav>

    <header class="row photo-on-head">
      <div class="col-sm-12 col-md-12">
        <div class="jumbotron head-photo my-0">
          <div class="photo-letters">
            <h1 class="display-4">Caleb Sherfick</h1>
            <p class="lead">Junior Software Developer</p>
          </div>
          <a class="btn btn-lg btn-color nav-text shadow" href="#" role="button">View Work</a>
        </div>
      </div>
    </header>







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

  .head-photo {
    background-image: url("../assets/federica-galli-449563-unsplash.jpg");
    background-size: 100%;
    width: 100%;
    background-position: center 95%;
    padding: 20vh;
    border-radius: 0px;
  }

  /* .photo-letters {  
  text-shadow: -1px 1px 2px;
} */

  .btn-color {
    background-color: #67747b;
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