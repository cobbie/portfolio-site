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
      <div class="about-grid-item item-1">Item 1</div>
      <div class="about-grid-item item-2">Item 2</div>
      <div class="about-grid-item item-3">Item 3</div>
      <div class="about-grid-item item-4">Item 4</div>
    </div>
  </div></div>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
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
  background-color: #EDEDED;
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
  text-align: center
}

.about-me>h1{
  font-size: 49.82px;
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
}

.about-grid-item{

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
</style>
