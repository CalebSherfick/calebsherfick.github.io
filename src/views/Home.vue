<template>
  <div class="container-fluid">

    <nav
      :class="$mq | mq({xs: 'navbar navbar-expand-lg navi row', sm: 'navbar navbar-expand-lg navi row', md: 'navbar sticky-top navbar-expand-lg navi row', lg: 'navbar sticky-top navbar-expand-lg navi row'})">
      <div class="col-12">
        <div class="row">
          <a :class="$mq | mq({xs: 'navbar-brand nav-text col-12', sm: 'navbar-brand nav-text col-12', md: 'navbar-brand nav-text col-2', lg: 'navbar-brand nav-text col-2'})"
            href="https://media.licdn.com/media-proxy/ext?w=800&h=800&f=n&hash=Cv%2F6Clm%2B4QB4KJQt3NxfQeb7iMU%3D&ora=1%2CaFBCTXdkRmpGL2lvQUFBPQ%2CxAVta5g-0R6jnhodx1Ey9KGTqAGj6E5DQJHUA3L0CHH05IbfPWi9fcCJKrfzpEAVf39TjQA7LOi1SWbmFI7tK4_sf94ki5DldZP5agYUbhl4lWdI"
            target="_blank">Caleb
            Sherfick
            Resume</a>
          <a :class="$mq | mq({xs: 'nav-item nav-link active nav-text col-6', sm: 'nav-item nav-link active nav-text col-6', md: 'nav-item nav-link active nav-text offset-5 col-1', lg: 'nav-item nav-link active nav-text offset-5 col-1'})"
            href="#about">About
            Me</a>
          <a :class="$mq | mq({xs: 'nav-item nav-link active nav-text col-6', sm: 'nav-item nav-link active nav-text col-6', md: 'nav-item nav-link active nav-text col-1', lg: 'nav-item nav-link active nav-text col-1'})"
            href="#skills">Skills</a>
          <a :class="$mq | mq({xs: 'nav-item nav-link active nav-text col-6', sm: 'nav-item nav-link active nav-text col-6', md: 'nav-item nav-link active nav-text col-1', lg: 'nav-item nav-link active nav-text col-1'})"
            href="#portfolio">Portfolio</a>
          <a :class="$mq | mq({xs: 'nav-item nav-link active nav-text col-6', sm: 'nav-item nav-link active nav-text col-6', md: 'nav-item nav-link active nav-text col-1', lg: 'nav-item nav-link active nav-text col-1'})"
            href="#contact">Contact</a>
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
            <a class="btn button btn-lg btn-text" href="#portfolio" role="button">View Work</a>
          </div>
        </div>
      </div>
    </header>

    <section class="row about" id="about">
      <div class="col-12">
        <div class="about-color">
          <div class="row align-items-center justify-content-center">
            <div class="col-12 flex-column text-center py-4">
              <h3 class="pb-1">ABOUT</h3>
            </div>
          </div>
          <div class="row justify-content-center">
            <div class="col-10">
              <p>I graduated from Boise State University with a Human Biology degree. In the midst of PA school
                interviews, I realized I
                wasn't passionate about the healthcare industry anymore and decided I needed a new challenge. This
                realization fueled the
                beginning of my journey in the field of Software Development. I started to study coding on my own and
                taught myself HTML
                and CSS using the many open source resources online. I quickly fell in love with coding and wanted to
                enhance my skills
                at a faster pace than I would be able to accomplish on my own. That is when I decided to quit my job to
                enroll in CodeWorks, where I have learned all the skills necessary to become a
                Full Stack Software
                Developer. With my studies at CodeWorks complete, I am now looking for work as a Full Stack Software
                Developer.</p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="row skills" id="skills">
      <div class="col-12 skills-bg">
        <div class="row align-items-center justify-content-center pt-4">
          <div class="col-12 text-center">
            <h3>SKILLS</h3>
          </div>
        </div>
        <div class="row">
          <!-- INSERT LANGUAGE IMAGE MODEL HERE -->
          <skill v-for="skill in skills" :skill="skill"></skill>
        </div>
      </div>
    </section>

    <section class="row portfolio" id="portfolio">
      <div class="col-12 portfolio-bg">
        <div class="row align-items-center justify-content-center pt-4">
          <div class="col-12 text-center">
            <h3>PORTFOLIO</h3>
          </div>
        </div>
        <div class="row justify-content-center  ">
          <!-- INSERT PROJECT IMAGE MOEDEL HERE -->
          <project v-for="project in projects" :project="project"></project>
        </div>
      </div>
    </section>

    <footer class="row contact" id="contact">
      <div class="col-12 pt-1 mt-3 foot-color">
        <div class="foot-color">
          <div class="row align-items-center justify-content-center">
            <a :class="$mq | mq({xs: 'col-12 text-center nav-text', sm: 'col-12 text-center nav-text', md: 'col-3 text-center nav-text', lg: 'col-3 text-center nav-text'})"
              href="tel:2082197635" target="_blank">
              <i
                :class="$mq | mq({xs: 'fas fa-phone fa-2x pt-4', sm: 'fas fa-phone fa-2x pt-4', md: 'fas fa-phone fa-2x pt-2', lg: 'fas fa-phone fa-2x pt-2'})"></i>
              <p
                :class="$mq | mq({xs: 'footer-words py-1', sm: 'footer-words py-1', md: 'footer-words my-0 py-1', lg: 'footer-words my-0 py-1'})">
                208.219.7635</p>
            </a>
            <a :class="$mq | mq({xs: 'col-12 text-center nav-text', sm: 'col-12 text-center nav-text', md: 'col-3 text-center nav-text', lg: 'col-3 text-center nav-text'})"
              href="mailto:calebsherfick@gmail.com" target="_blank">
              <i
                :class="$mq | mq({xs: 'fas fa-envelope fa-2x pt-1', sm: 'fas fa-envelope fa-2x pt-1', md: 'fas fa-envelope fa-2x pt-2', lg: 'fas fa-envelope fa-2x pt-2'})"></i>
              <p
                :class="$mq | mq({xs: 'footer-words py-1', sm: 'footer-words py-1', md: 'footer-words my-0 py-1', lg: 'footer-words my-0 py-1'})">
                calebsherfick@gmail.com
              </p>
            </a>
            <a :class="$mq | mq({xs: 'col-12 text-center nav-text', sm: 'col-12 text-center nav-text', md: 'col-3 text-center nav-text', lg: 'col-3 text-center nav-text'})"
              href="https://media.licdn.com/media-proxy/ext?w=800&h=800&f=n&hash=Cv%2F6Clm%2B4QB4KJQt3NxfQeb7iMU%3D&ora=1%2CaFBCTXdkRmpGL2lvQUFBPQ%2CxAVta5g-0R6jnhodx1Ey9KGTqAGj6E5DQJHUA3L0CHH05IbfPWi9fcCJKrfzpEAVf39TjQA7LOi1SWbmFI7tK4_sf94ki5DldZP5agYUbhl4lWdI"
              target="_blank">
              <i
                :class="$mq | mq({xs: 'fas fa-file-alt fa-2x pt-1', sm: 'fas fa-file-alt fa-2x pt-1', md: 'fas fa-file-alt fa-2x pt-2', lg: 'fas fa-file-alt fa-2x pt-2'})"></i>
              <p
                :class="$mq | mq({xs: 'footer-words py-1', sm: 'footer-words py-1', md: 'footer-words my-0 py-1', lg: 'footer-words my-0 py-1'})">
                Resume</p>
            </a>
          </div>
        </div>
      </div>
    </footer>



    <!-- :class="$mq | mq({xs: '', sm: '', md: '', lg: ''})" -->


  </div>
</template>

<script>
  import mySql from '@/assets/1200px-MySQL.svg.png'
  import bootstrap from '@/assets/bootstrap-logo-vector-png-bootstrap-logo-vector-300.png'
  import cs from '@/assets/c-logo.png'
  import css from '@/assets/css3-logo-png-transparent.png'
  import git from '@/assets/Git-Logo-2Color.png'
  import html from '@/assets/HTML5_Logo_512.png'
  import js from '@/assets/logo-javascript-png-javascript-tutorials-400.png'
  import mongoDb from '@/assets/logo-mongodb-png-mongodb-is-one-of-several-database-types-to-arise-in-the-mid-2000s-under-the-nosql-banner-instead-of-using-tables-and-rows-as-in-relational-databases-300.png'
  import vue from '@/assets/logo.png'
  import node from '@/assets/nodejs-new-pantone-black.png'

  import inspire from '@/assets/Inspire.png'
  import bugReport from '@/assets/BugReport.png'
  import billboards from '@/assets/Billboards.png'
  import poplarWide from '@/assets/PoplarWide.jpg'
  import poplar from '@/assets/Poplar.jpg'

  import Skill from "@/components/Skill.vue"
  import Project from "@/components/Project.vue"

  export default {
    name: 'home',
    data() {
      return {
        skills: [
          { url: mySql, id: "mySql" },
          { url: bootstrap, id: "bootstrap" },
          { url: cs, id: "cs" },
          { url: css, id: "css" },
          { url: git, id: "git" },
          { url: html, id: "html" },
          { url: js, id: "js" },
          { url: mongoDb, id: "mongoDb" },
          { url: vue, id: "vue" },
          { url: node, id: "node" }
        ],
        projects: [
          { url: inspire, id: "inspire", title: "Inspire", link: "https://calebsherfick.github.io/inspire/", desc: "Vanilla JavaScript homepage application. Includes a todo list and implements multiple APIs to draw in weather, photo, and a quote per page load." },
          { url: bugReport, id: "bugReport", title: "Bug Report", link: "https://calebsherfick.github.io/bug-report/", desc: "Created using Vue.js allowing users to report bugs, view details, post/flag comments, and close bugs." },
          { url: billboards, id: "billboards", title: "Billboards", link: "https://lnkd.in/eMUcpjK", desc: "(TEST ACCOUNT: EMAIL= test@test.com | PASSWORD= test123) Full Stack application, which allows users to get organized by adding lists to boards. Users are able to drag and drop tasks to different lists on the board. Incorporates user authentication, allowing users to sign in for private boards." },
          { url: poplarWide, id: "poplarWide", title: "Poplar", link: "", desc: "(COMING SOON, CURRENTLY UNHOSTED) Full Stack polling application which allows users to vote on posts and express their opinion based on this/that and yes/no questions. Incorporates sockets to provide a unique chatroom for every post, as well as a photo cropping/ uploading tool and user authentication." },
          // { url: poplar, id: "poplar", title: "Poplar", link: "", desc: "(COMING SOON, CURRENTLY UNHOSTED) Full Stack polling application which allows users to vote on posts and express their opinion based on this/that and yes/no questions. Incorporates sockets to provide a unique chatroom for every post, as well as a photo cropping/ uploading tool and user authentication." },
        ]
      }
    },
    computed: {
    },
    components: {
      Skill,
      Project
    }
  }
</script>

<style>
  /* * {
    outline: 1px red solid;
  } */

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

  .nav-text:hover {
    color: white;
    text-shadow: 0px 0px 2px white;
  }

  .nav-text:active {
    color: rgb(187, 187, 187);
    text-shadow: 0px 0px 0px black;
  }

  .button {
    background-color: #67747b;
    border: none;
    border-radius: 50px;
    color: #FFF;
    padding: 10px 50px;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 18px;
  }

  .button:hover {
    background-color: #70848f;
  }

  .button:active {
    background-color: #576770;
  }

  .btn-text {
    color: #f4fffd;
  }

  .btn-text:hover {
    color: #f4fffd;
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

  .about {
    margin-left: 0px;
    margin-right: 0px;
    margin-bottom: 32px;
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
  }

  .footer-words {
    font-size: 1.3em;
  }

  .project-text {
    color: #f4fffd;
    text-shadow: -1px 1px 2px;
  }
</style>