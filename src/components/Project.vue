<template>
  <div
    :class="$mq | mq({xs: 'col-12 imgContainer mt-3', sm: 'col-12 imgContainer mt-3', md: 'col-6 imgContainer mt-3', lg: 'col-6 imgContainer mt-3'})">
    <a :href="project.link" target="_blank">
      <img :src="project.url"
        :class="$mq | mq({xs: 'project-img', sm: 'project-img', md: 'project-img', lg: 'project-img'})">
      <div
        :class="$mq | mq({xs: 'overlay-mobile row align-items-start', sm: 'overlay-mobile row align-items-start', md: 'overlay row align-items-start', lg: 'overlay row align-items-start'})">
        <div class="col-12 text-div d-flex justify-content-center align-items-end">
          <div
            :class="$mq | mq({xs: 'text-mobile title-text-mobile', sm: 'text-mobile title-text-mobile', md: 'text title-text', lg: 'text title-text'})">
            {{project.title}}</div>
        </div>
        <div class="col-12 text-div d-flex justify-content-center align-items-start">
          <div :class="$mq | mq({xs: 'text-mobile', sm: 'text-mobile', md: 'text desc-text', lg: 'text desc-text'})">
            {{project.desc}}}
          </div>
        </div>
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
  .project-img {
    width: 100%;
    height: auto;
    display: block;
  }

  .overlay {
    position: absolute;
    /* top: 0; */
    bottom: 0;
    left: 0;
    right: 0;
    margin-left: 15px;
    height: 0;
    width: 95.5%;
    overflow: hidden;
    /* opacity: 0; */
    transition: .5s ease;
    background-color: rgba(0, 0, 0, 0.432);
  }

  .overlay-mobile {
    position: absolute;
    /* top: 0; */
    bottom: 0;
    left: 0;
    right: 0;
    margin-left: 15px;
    height: 100%;
    width: 93%;
    overflow: hidden;
    /* opacity: 0; */
    transition: .5s ease;
    background-color: rgba(0, 0, 0, 0.432);
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