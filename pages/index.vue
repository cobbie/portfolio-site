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
    <h1>What I like to do</h1>
    
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
}

.about-me>h1{
  font-size: 49.82px;
  font-weight: normal
}
</style>
