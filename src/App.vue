<template>
  <!-- navbar -->
  <div class="sticky-top">
    <nav class="navbar navbar-expand-md navbar-dark">
      <div class="container-fluid">
        <a href="#" class="brand">AC</a>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarSupportedContent"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav ms-auto">
            <li class="nav-item mx-2">
              <a class="nav-link" href="#about">About</a>
            </li>
            <li class="nav-item mx-2">
              <a class="nav-link" href="#projects">Projects</a>
            </li>
            <li class="nav-item mx-2 mb-md-0 mb-2">
              <a class="nav-link" href="#contact">Contact</a>
            </li>
          </ul>
          <a href="" class="button-link external-link mx-2 mb-md-0">Resume</a>
        </div>
      </div>
    </nav>
  </div>

  <div class="container-fluid">
    <div class="row">
      <div class="col col-1 d-none d-md-flex justify-content-center">
        <div class="sidebar ml-5">
          <div>
            <a class="push-bottom" href="https://github.com/arenclissold"><git-hub-icon /></a>
          </div>
          <div>
            <a href="https://www.linkedin.com/in/arenclissold/"><linked-in-icon /></a>
          </div>
          <div class="side-line"></div>
        </div>
      </div>
      <div class="col mx-4">
        <section>
          <h3>Hi, my name is</h3>
          <h1>Aren</h1>
          <h2>I build things for the web</h2>
        </section>
        <section>
          <div class="sub-heading">
            <h2 id="about">About</h2>
            <div class="line"></div>
          </div>
          <div class="container">
            <div class="row justify-content-center">
              <div class="col-lg">
                <p>
                  Lorem ipsum, dolor sit amet consectetur adipisicing elit. Totam sunt unde aliquid
                  soluta maiores voluptatem fugiat excepturi, eveniet, expedita ratione magni culpa
                  optio adipisci omnis, voluptatum facilis aliquam cum nesciunt.
                  <br /><br />
                  Lorem ipsum dolor sit amet consectetur adipisicing elit. Ducimus hic, repudiandae
                  ad iusto atque impedit fugiat amet numquam nihil laboriosam nulla pariatur soluta
                  dignissimos minus perferendis? Laborum optio quos tempora.
                </p>
                <ul class="skill-list">
                  <li v-for="(skill, index) in skills" :key="skill._id">
                    {{ skill }}
                    <div v-if="index != skills.length - 1" class="list-line"></div>
                  </li>
                </ul>
              </div>
              <div class="col-lg">
                <div class="flex-center">
                  <div class="photo-parent">
                    <img
                      class="shadow-lg"
                      src="./assets/test_pic.jpeg"
                      alt="profile picture"
                      id="photo"
                    />
                    <div class="photo-border"></div>
                  </div>
                </div>
              </div>
            </div>
            <span id="projects"></span>
          </div>
        </section>

        <section>
          <div class="sub-heading">
            <h2>Things I've Built</h2>
            <div class="line"></div>
          </div>
          <div class="project-cards">
            <div class="project-card mt-5">
              <div class="project-opacity"></div>
              <img class="project-img" src="./assets/dayt_image.jpeg" alt="camping" />
              <div class="project-body project-body-right">
                <h3>Dayt</h3>
                <p class="project-description project-description-right shadow-lg">
                  Dayt is a travel planning web app designed to make planning your next trip simple and
                  easy while providing authentic experiences recommended by locals. Featuring geocoding, image upload, authentication and front end npm packages for a smooth user experience.
                </p>
                <p class="project-technologies">
                  Ruby On Rails | Postgresql | JavaScript | SCSS | REST
                </p>
                <div class="project-links">
                  <a href="https://github.com/hwalk1/dayt_app"><git-hub-icon /></a>
                  <a href="https://www.dayt.travel" class="project-link"><project-link-icon /></a>
                </div>
              </div>
            </div>
            <div class="project-card">
              <div class="project-opacity project-opacity-left"></div>
              <img
                class="project-img project-img-left"
                src="./assets/gig-fox.png"
                alt="camping"
              />
              <div class="project-body">
                <h3>Camping App</h3>
                <p class="project-description shadow-lg">
                  A web app for posting and booking venues around Melbourne. Post your own venue and see it appear on the map. Featuring geocoding, image upload, authentication and authorisation.
                </p>
                <p class="project-technologies">Ruby On Rails | Postgresql | JavaScript | SCSS | REST</p>
                <div class="project-links">
                  <a href="https://github.com/hwalk1/gigfox"><git-hub-icon /></a>
                  <a href="https://gig-fox.herokuapp.com/" class="project-link"><project-link-icon /></a>
                </div>
              </div>
            </div>
            <div class="project-card">
              <div class="project-opacity"></div>
              <img class="project-img" src="./assets/hiking_pic.jpg" alt="camping" />
              <div class="project-body project-body-right">
                <h3>Coming Soon - Camping App</h3>
                <p class="project-description project-description-right shadow-lg">
                  A modern application to find, share and review camping spots. Helping you discover those magical camping spots and miss the so-so ones.
                </p>
                <p class="project-technologies">Express | MongoDB | mongoose | Node | REST</p>
                <div class="project-links">
                  <a href="https://github.com/arenclissold/open-trivia"><git-hub-icon /></a>
                </div>
              </div>
            </div>
          </div>
        </section>

        <section class="centered margin-bottom">
          <div class="sub-heading center-content">
            <div class="small-line"></div>
            <h2 id="contact">Get in Touch</h2>
            <div class="small-line"></div>
          </div>
          <p class="last">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Animi, corrupti laboriosam
            architecto incidunt aliquid reprehenderit facilis, aliquam illum voluptatibus suscipit
            eum dolorem rerum ratione odio assumenda beatae laudantium impedit nostrum.
          </p>
          <a href="mailto:arenclissold@gmail.com" class="hello-button external-link">Say Hello</a>
        </section>
        <footer>
          <div class="footer-links">
            <a href="https://github.com/arenclissold"><git-hub-icon /></a>
            <a href="https://www.linkedin.com/in/arenclissold/"><linked-in-icon /></a>
          </div>
        </footer>
      </div>
      <div class="col col-1 d-none d-md-flex justify-content-center">
        <div class="sidebar">
          <div class="sideways">
            <a class="sidebar-link" href="mailto:arenclissold@gmail.com">arenclissold@gmail.com</a>
          </div>
          <div class="side-line"></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import GitHubIcon from "../components/GitHubIcon.vue";
import ProjectLinkIcon from "../components/ProjectLinkIcon.vue";
import LinkedInIcon from "../components/LinkedInIcon.vue";
const skills = [
  "Ruby",
  "Ruby on Rails",
  "JavaScript",
  "DOM Manipulation",
  "HTML5",
  "CSS3",
  "Git",
  "GitHub",
  "MongoDB",
  "Node",
  "Express",
  "AJAX",
  "REST APIs",
];
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Roboto+Mono&display=swap");

:root {
  --primary-color: #4cc9f0;
  --secondary-color: #aeb9df;
  --line-color: #2f3957;
}

#app {
  margin: 0;
  background-color: #0a1128;
  color: var(--secondary-color);
  font-family: "Roboto", sans-serif;
}

.tagcloud {
  font-size: 20px;
  font-weight: 650;
  margin-left: 30%;
}
.tagcloud--item:hover {
  color: #36454f;
}

.external-link {
  text-decoration: none;
  color: var(--primary-color);
}

.centered {
  text-align: center;
}

.center-content {
  justify-content: center;
}

.relative {
  position: relative;
}

.navbar {
  box-shadow: 0 8px 32px 0 rgba(0, 0, 0, 0.3);
  backdrop-filter: blur(4px);
  z-index: 10;
}

.nav-link {
  color: rgb(178, 188, 190) !important;
}

.sticky-top {
  position: fixed;
}

.brand {
  height: 40px;
  width: 35px;
  margin: 10px;
}

.sidebar {
  position: fixed;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: end;
  height: 100%;
  bottom: 0px;
  width: 100px;
}

.side-line {
  height: 200px;
  width: 2px;
  background: var(--line-color);
  margin-top: 1em;
}

.push-bottom {
  position: relative;
  bottom: 20px;
}

.sidebar-link {
  text-decoration: none;
  color: currentColor;
  transition: 0.5s;
}

.sidebar-link:hover {
  color: var(--primary-color);
}

.sideways {
  transform: rotate(270deg);
  margin-bottom: 5em;
}

section {
  margin-top: 7em;
}

.button-link {
  border: solid var(--primary-color);
  border-radius: 5px;
  padding: 0.5em 1em;
  transition: 0.5s;
  margin: 0.5em;
}

.button-link:hover {
  color: var(--primary-color);
  background-color: #4ccaf02b;
}

h3 {
  font-family: "Roboto Mono", monospace;
  color: var(--primary-color);
  font-size: 16px !important;
}

.line {
  height: 1px;
  width: 50%;
  background: var(--line-color);
  margin: 0em 2em;
}

.small-line {
  height: 1px;
  width: 20%;
  background: var(--line-color);
  margin: 0em 2em;
}

.sub-heading {
  display: flex;
  align-items: center;
  width: 100%;
  margin-bottom: 0.5em;
}
.skill-list {
  margin-top: 2em;
  width: 80%;
}

.skill-list > li {
  display: inline;
}

.list-line {
  display: inline-block;
  width: 3px;
  height: 3px;
  background-color: white;
  margin: 0px 0.5em 0.2em 0.5em;
  transform: rotate(45deg);
}

.photo-parent {
  position: relative;
}

.photo-border {
  border: 0.2em solid var(--primary-color);
  border-radius: 0.4em;
  top: 1.5em;
  left: 1.5em;
  height: 20em;
  width: 20em;
  position: absolute;
  z-index: 0;
  transition: 0.5s;
}

#photo {
  height: 20em;
  width: 20em;
  border-radius: 0.2em;
  z-index: 1;
  position: relative;
}

#photo:hover ~ .photo-border {
  top: 1em;
  left: 1em;
}

.flex-center {
  display: flex;
  justify-content: center;
  margin: 2em;
}

.project-cards {
  display: flex;
  flex-direction: column;
}

.project-card {
  position: relative;
  height: 20em;
  width: auto;
  box-shadow: 0px 8px 24px #00032c4f;
  margin-top: 7em;
}

.project-body {
  z-index: 2;
  position: relative;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  box-shadow: inset darkblue;
  padding: 1em;
  width: 100%;
  height: 100%;
}

.project-img {
  height: 100%;
  width: 100%;
  position: absolute;
  z-index: 0;
  border-radius: 5px;
  object-fit: cover;
  object-position: top;
}

.project-opacity {
  height: 100%;
  width: 100%;
  position: absolute;
  z-index: 1;
  background-color: #001f54;
  opacity: 0.8;
  border-radius: 5px;
}

@media (min-width: 992px) {
  .project-body-right {
    text-align: right;
    width: 55%;
    float: right;
  }

  .project-body {
    width: 55%;
  }

  .project-opacity:hover {
    background-color: rgba(0, 0, 0, 0);
  }

  .project-img {
    width: 60%;
  }

  .project-img-left {
    width: 60%;
    right: 0px;
  }

  .project-opacity {
    width: 60%;
    transition: background-color 1s, width 0s;
    opacity: 0;
  }

  .project-opacity-left {
    width: 60%;
    right: 0px;
  }

  .project-description-right {
    align-self: flex-end;
  }

  .project-description {
    background-color: #001f54;
    padding: 30px;
    border-radius: 5px;
  }
}

.link-icon {
  width: 2em;
  height: 2em;
  color: var(--secondary-color);
  margin-right: 0.5em;
  transition: 0.5s;
}

.link-icon:hover {
  color: var(--primary-color);
}

.last-p {
  width: 60%;
}

.hello-button {
  border: solid var(--primary-color);
  display: inline-block;
  border-radius: 5px;
  padding: 1rem 2rem;
  transition: 0.5s;
}

.hello-button:hover {
  color: var(--primary-color);
  background-color: #4ccaf02b;
}

.linkedin {
  width: 2em;
  height: 2em;
  stroke: var(--secondary-color);
  transition: 0.5s;
}

.footer-links {
  display: flex;
  justify-content: center;
  margin: 2em 0em;
  gap: 1em;
}

.mail {
  stroke: var(--secondary-color);
}
</style>
