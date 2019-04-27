<template>
  <div class="whole-project px-0"
    :class="$mq | mq({xs: 'col-12 m-1', sm: 'col-12 m-1', md: ' col-5 mt-3', lg: ' col-5 mt-3'})">
    <a :href="project.link" target="_blank">
      <img class="projectImg" :src="project.url">

      <div
        :class="$mq | mq({xs: 'overlay-mobile-top', sm: 'overlay-mobile-top', md: 'overlay-top', lg: 'overlay-top'})">
        <div class="row">
          <div class="col-12 d-flex align-items-center justify-content-center">
            <p class="project-title" style="font-weight:750;">{{project.title}}</p>
          </div>
        </div>
      </div>

      <div
        :class="$mq | mq({xs: 'overlay-mobile-bottom', sm: 'overlay-mobile-bottom', md: 'overlay-bottom', lg: 'overlay-bottom'})">
        <p
          :class="$mq | mq({xs: 'view-details-mobile', sm: 'view-details-mobile', md: 'view-details', lg: 'view-details'})">
          {{project.desc}}</p>
      </div>

    </a>
  </div>
</template>

<script>
  export default {
    name: "project",
    props: ["project"],
    data() {
      return {};
    },
    computed: {},
    methods: {},
    components: {}
  };
</script>

<style>
  .whole-project {
    position: relative;
    width: 100%;
  }

  .projectImg {
    display: block;
    width: 100%;
    height: auto;
  }

  .projectImg:hover {
    cursor: pointer;
  }

  .project-title {
    color: white;
    width: 90%;
    text-align: center;
    font-size: 18px;
  }

  .view-details {
    color: white;
    width: 90%;
    position: absolute;
    text-align: center;
    font-size: 18px;
    transform: translate(-50%, -50%);
    top: 40%;
    left: 50%;
  }

  .view-details-mobile {
    color: white;
    width: 90%;
    position: absolute;
    text-align: center;
    font-size: 13px;
    transform: translate(-50%, -50%);
    top: 50%;
    left: 50%;
  }

  .overlay-bottom {
    position: absolute;
    bottom: 0;
    left: 0;
    right: 0;
    background-color: rgba(51, 51, 51, 0.568);
    overflow: hidden;
    width: 100%;
    height: 0;
    transition: .5s ease;
  }

  .overlay-top {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    background-color: #2d3142;
    overflow: hidden;
    width: 100%;
    height: 0;
    transition: .5s ease;
  }

  .whole-project:hover .overlay-top {
    height: 10%;
    cursor: pointer;
  }

  .whole-project:hover .overlay-bottom {
    height: 90%;
    cursor: pointer;
  }

  .overlay-mobile-bottom {
    position: absolute;
    bottom: 0;
    left: 0;
    right: 0;
    background-color: rgba(51, 51, 51, 0.568);
    overflow: hidden;
    width: 100%;
    height: 85%;
    transition: .5s ease;
  }

  .overlay-mobile-top {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    background-color: #2d3142;
    overflow: hidden;
    width: 100%;
    height: 15%;
    transition: .5s ease;
  }



















  .imgContainer {
    position: relative;
    width: 50%;
  }

  .imgContainer:hover .overlay {
    /* opacity: 1; */
    height: 100%;
  }

  .text {
    color: white;
    /* font-size: 20px; */
    /* position: absolute;
    top: 50%;
    left: 50%; */
    height: 90%;
    width: 80%;
    /* -webkit-transform: translate(-50%, -50%);
    -ms-transform: translate(-50%, -50%);
    transform: translate(-50%, -50%); */
    text-align: center;
  }

  .text-mobile {
    color: white;
    /* font-size: 20px; */
    /* position: absolute;
    top: 50%;
    left: 50%; */
    height: 90%;
    width: 100%;
    /* -webkit-transform: translate(-50%, -50%);
    -ms-transform: translate(-50%, -50%);
    transform: translate(-50%, -50%); */
    text-align: center;
  }

  .title-text {
    font-size: 2em;
  }

  .title-text-mobile {
    font-size: 1.5em;
  }

  .desc-text {
    font-size: 1.3em;
  }


  /* .text-div {
    height: 100vh;
    width: 100vh;
  } */
</style>