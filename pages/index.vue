<template>
  <div>
    <div class="container">
      <h1>Cobbie Quintos</h1>
      <div id="logos">
        <a href="https://www.github.com/cobbie" target="_blank">
          <img src="~/assets/github.svg" />
        </a>
        <a href="https://www.twitter.com/cobbiequintos" target="_blank">
          <img src="~/assets/twitter.svg" />
        </a>
        <a href="https://www.linkedin.com/in/cobbie-quintos-01b536159/" target="_blank">
          <img src="~/assets/linkedin.svg" />
        </a>
      </div>
      <div id="links">
        <a @click="scroll('about-me')">About</a> •
        <a @click="scroll('works')">Projects</a> •
        <a href="https://drive.google.com/file/d/1kKJQSFDGJa_Y5FxTRjn-E4Q5Dr4MKnO-/view" class="resume-link" target="_blank">Resume</a>
      </div>
    </div>
    <div class="about-me">
      <div class= "screws-div">
        <img src="~/assets/screw.svg" class="rotate-neg test screw" alt="screw">
      <img src="~/assets/screw.svg" class="rotate test2 screw" alt="screw">
      </div>
      <div class= "screws-div2">
        <img src="~/assets/screw.svg" class="rotate-neg test screw" alt="screw">
      <img src="~/assets/screw.svg" class="rotate test2 screw" alt="screw">
      </div>
      <div class= "screws-div3">
        <img src="~/assets/screw.svg" class="rotate-neg test screw" alt="screw">
      <img src="~/assets/screw.svg" class="rotate test2 screw" alt="screw">
      </div>
      
      <h1 class="about-header">
        <a name="about">What I like to do</a>
      </h1>

      <div class="about-grid">
        <div class="about-grid-item item-1">
          <img class="about-item-img" src="~/assets/idea.svg" alt />
          <h1 class="about-item-header">
            <span id="code">Code</span> Learn & build things
          </h1>
          <p
            class="about-item-p"
          >I developed a passion for coding ever since I entered college. Dealing mostly with front-end development, my main experience lies with JavaScript, VueJS, and Node, but I also consider myself to be a pretty okay Python programmer.</p>
        </div>
        <div class="about-grid-item item-2">
          <img class="about-item-img" src="~/assets/magichat.svg" alt />
          <h1 class="about-item-header">
            <span id="code">Games</span> Adventures
          </h1>
          <p
            class="about-item-p"
          >One of the things I'm most thankful for is that I was lucky enough to grow up in a time where gaming (and technology in general) really started to take off. Some of my favorite titles/franchises are Overwatch, Apex Legends, Horizon Zero Dawn, Call of Duty, and Pokemon.</p>
        </div>
        <div class="about-grid-item item-3">
          <img class="about-item-img" src="~/assets/handshake.svg" alt />
          <h1 class="about-item-header">
            <span id="code">Networking</span> Meeting people
          </h1>
          <p class="about-item-p">
            I'm an introvert. But
             <!-- I've had the privilege of being able to go on two life-changing experiences abroad
            during my stay in college. Among the many things I learned in these adventures, here's one of the most valuable lessons: there
            are so many things you can only learn by meeting and talking to other people, especially from different backgrounds and places. -->
          </p>
        </div>
        <div class="about-grid-item item-4">
          <img class="about-item-img" src="~/assets/idea.svg" alt />
          <h1 class="about-item-header">
            <span id="code">Lorem</span> Ipsum
          </h1>
          <p class="about-item-p">
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur
            
          </p>
        </div>
      </div>
    </div>
    <div class="works">
      <h1 class="project-header-main">Projects</h1>
      <h3 class="resume">
        You can also take a look at my
        <u>resume</u>.
      </h3>
      <div class="proj-grid">
        <project
          class="proj-grid-item proj-item-1"
          title="Marawi Interactive Website"
          org="The GUIDON"
          desc="Using a static site generator framework called Gridsome and Vue.js, I wrote code that was "
        ></project>
        <project class="proj-grid-item"></project>
        <project class="proj-grid-item"></project>
        <project class="proj-grid-item"></project>
        <project class="proj-grid-item"></project>
        <project class="proj-grid-item"></project>
      </div>
    </div>

    <footer>
      <p>Wanna connect/inquire, collaborate, have a cup of coffee, or play some Apex legends/Pokemon? You can shoot me an email at cobbiequintos@gmail.com, send me a LinkedIn message, or tweet me @cobbiequintos.</p>
    </footer>
  </div>
</template>

<script>
import Logo from "~/components/Logo.vue";
import Project from "~/components/Project.vue";

export default {
  components: {
    Logo,
    Project
  },
  methods: {
    scroll: function(id) {
      document
        .getElementsByClassName(id)[0]
        .scrollIntoView({ behavior: "smooth", block: "center" });
    }
  }
};
</script>

<style>
@import url("https://fonts.googleapis.com/css?family=Noto+Sans&display=swap");
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  flex-direction: column;
  background-color: #1a2859;
  font-family: "Noto Sans", sans-serif;
  width: 100%;
  color: #ffffff;
}
.container > h1 {
  font-size: 88.82px;
}
#logos {
  display: block;
  width: 30vw;
  margin-top: 57px;
}

#logos > a {
  display: inline-block;
  padding: 20px;
  transition: all 0.2s;
  transform-origin: 50% 50%;
}
#logos > a:hover {
  transform: scale(1.2);
  cursor: pointer;
}

#logos > img:hover {
  transform: scale(1.2);
  cursor: pointer;
}

#links {
  font-size: 25px;
  margin-top: 66.27px;
}

.about-me {
  background-color: #e8e8e8;
  color: #1a2859;
  padding-top: 10vh;
  margin: 0 auto;
  display: block;
  text-align: center;
  height: auto;
  padding-top: 80px;
  padding-bottom: 80px;
}

.about-header {
  margin: 0 auto;
  display: block;
  width: 90vw;
  text-align: center;
  font-size: 40.82px;
  font-weight: normal;
}

.about-grid {
  display: grid;
  margin: 0 auto;
  margin-top: 68px;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: 1fr 1fr;
  grid-template-areas:
    "first-item second-item"
    "third-item fourth-item";
  width: 80vw;
  height: 80vh;
  color: black;
}

.about-grid-item {
  display: grid;
  grid-template-columns: 20% 5% 75%;
  grid-template-rows: 20% 80%;
  grid-template-areas:
    "image . header "
    ". . body ";
}

.about-grid-item > h1 {
  font-weight: normal;
}
.about-item-img {
  grid-area: image;
  justify-self: right;
  align-self: right;
}
.about-item-p {
  grid-area: body;
  text-align: left;
  padding-top: 10px;
  line-height: 22px;
  font-size: 15px;
}
.about-item-header {
  grid-area: header;
  text-align: left;
  font-size: 30px;
}
#code {
  text-decoration: line-through;
}

.resume {
  margin: 0 auto;
  color: white;
  font-size: 16px;
  text-align: center;
  padding-top: 12px;
  font-weight: normal;
}

.works {
  background-color: #1a2859;
  height: auto;
  padding-top: 80px;
  padding-bottom: 100px;
}
.project-header-main {
  color: white;
  font-weight: normal;
  font-size: 40.82px;
  padding-top: 60px;
  text-align: center;
}
.proj-grid {
  display: grid;
  margin: 0 auto;
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: 1fr 1fr;
  width: 90vw;
  padding-top: 80px;
  row-gap: 5em;;
}
.proj-grid-item {
}

footer {
  height: 200px;
  background-color: #e8e8e8;
  display: flex;
  justify-content: center;
  vertical-align: middle;
  align-items: center;
  height: 20vh;
}

footer > p {
  width: 80vw;
  font-family: Noto Sans;
  font-style: normal;
  font-weight: normal;
  font-size: 18px;
  line-height: 25px;
}
u,
a {
  cursor: pointer;
}

a:hover {
  font-weight: bold;
}

.resume-link{
  text-decoration: none;
  color: white;
}

@keyframes rotating{
  from{
transform: rotate(0deg);
  }

  to{
transform: rotate(360deg);
  }
}

@keyframes negative-rotating{
  from{
    transform: rotate(0deg)
  }
  to{
    transform: rotate(-360deg)
  }
}
.rotate{
  animation: rotating 4s linear infinite
}

.rotate-neg{
  animation: negative-rotating 4s linear infinite;
}

.screws-div{
  margin-top: 20px;
  position: absolute;
  width: 100%;
  display: flex;
  justify-content: space-between
}
.test{
  margin-left: 40px;
}

.test2{
  margin-right: 40px
}

.screws-div2{
  margin-top: 300px;
  position: absolute;
  width: 100%;
  display: flex;
  justify-content: space-between
}

.screws-div3{
  margin-top: 580px;
  position: absolute;
  width: 100%;
  display: flex;
  justify-content: space-between
}
.screw{
  height: auto;
  width: 40px;
}
</style>
