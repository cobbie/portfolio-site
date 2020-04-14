<template>
  <div><div class="container">
  <h1>Cobbie Quintos</h1>
  <div id="logos">
  <img src="~/assets/github.svg">
  <img src="~/assets/twitter.svg">
  <img src="~/assets/linkedin.svg">
  </div>
  <div id="links">
  <span>Resume</span> • <span>Works</span> • <span>Ewan</span>
  </div>
  </div>
  <div class="about-me">
    <h1 class="about-header">What I like to do</h1>
    <div class="about-grid">
      <div class="about-grid-item item-1">
        <img class="about-item-img" src="~/assets/idea.svg" alt="">
        <h1 class="about-item-header"><span id="code">Code</span> Learn & build things</h1>
        <p class="about-item-p">I developed a passion for coding ever since I entered college. Dealing mostly with front-end development, my main experience lies with JavaScript, VueJS, and Node, but I also consider myself to be a pretty okay Python programmer.</p>
      </div>
      <div class="about-grid-item item-2"><img class="about-item-img" src="~/assets/magichat.svg" alt="">
        <h1 class="about-item-header"><span id="code">Games</span> Adventures</h1>
        <p class="about-item-p">One of the things I'm most thankful for is that I was lucky enough to grow up in a time where gaming (and technology in general) really started to take off. Some of my favorite titles/franchises are Overwatch, Apex Legends, Horizon Zero Dawn, Call of Duty, and Pokemon.</p></div>
      <div class="about-grid-item item-3"><img class="about-item-img" src="~/assets/handshake.svg" alt="">
        <h1 class="about-item-header"><span id="code">Networking</span> Meeting people</h1>
        <p class="about-item-p">I'm an introvert. But I've had the privilege of being able to go on two life-changing experiences abroad
          during my stay in college. Among the many things I learned in these adventures, here's one of the most valuable lessons: there 
          are so many things you can only learn by meeting and talking to other people, especially from different backgrounds and places.</p></div>
      <div class="about-grid-item item-4"><img class="about-item-img" src="~/assets/idea.svg" alt="">
        <h1 class="about-item-header"><span id="code">Code</span> Build things</h1>
        <p class="about-item-p"></p></div>
    </div>
  </div>
  <div class="works">
    <h1 class="project-header-main">Projects</h1>
    <div class="proj-grid">
      <project class="proj-grid-item proj-item-1" title="Marawi Interactive Website" org="The GUIDON" desc="Using a static site generator framework called Gridsome and Vue.js, I wrote code that was "></project>
      <project class="proj-grid-item"></project>
      <project class="proj-grid-item"></project>
      <project class="proj-grid-item"></project>
      <project class="proj-grid-item"></project>
      <project class="proj-grid-item"></project>
    </div>
  </div>
  
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import Project from '~/components/Project.vue'

export default {
  components: {
    Logo,
    Project
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Noto+Sans&display=swap');
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  flex-direction: column;
  background-color: #1A2859;
  font-family: 'Noto Sans', sans-serif;
  width: 100%;
  color: #FFFFFF;
}
.container>h1{
  font-size: 88.82px;
}
#logos{
  display: block;
  width: 30vw;
  margin-top: 57px;
}

#logos>img{
  padding: 20px;
  transition: all 0.2s;
  transform-origin: 50% 50%;

}

#logos>img:hover{
  transform: scale(1.2);
  cursor: pointer;
}

#links{
  font-size: 25px;
  margin-top: 66.27px;
}

.about-me{
  background-color: #E8E8E8;
  color: #1A2859;
  padding-top: 10vh;
  margin: 0 auto;
  display: block;
    text-align: center;
}

.about-header{
    margin: 0 auto;
  display: block;
  width: 90vw;
  text-align: center;
font-size: 40.82px;
  font-weight: normal
}

.about-grid{
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

.about-grid-item{
  display: grid;
  grid-template-columns: 20% 5% 75%;
  grid-template-rows: 20% 80%;
  grid-template-areas: 
  "image . header " 
  ". . body ";
}

.item-1{
  /* grid-area: first-item; */
  /* grid-column-start: 1;
  grid-column-end: 2;
  grid-row-start: 1;
  grid-row-end: 2; */
}

.item-2{
  /* grid-area: second-item */
}

.item-3{
  /* grid-area: third-item */
}
.item-4{
  /* grid-area: fourth-item */
}

.about-grid-item>h1{
  font-weight: normal;
}
.about-item-img{
  grid-area: image;
  justify-self: right;
  align-self: right;
}
.about-item-p{
  grid-area: body;
  text-align: left;
  padding-top: 10px;
  line-height: 22px;
  font-size: 15px;
}
.about-item-header{
  grid-area: header;
  text-align: left;
  font-size: 30px;

}
#code{
  text-decoration: line-through
}

.works{
  background-color: #1A2859;
}
.project-header-main{
  color: white;
  font-weight: normal;
  font-size: 40.82px;
  padding-top: 60px;
text-align: center;
}
</style>
