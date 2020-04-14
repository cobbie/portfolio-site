<template>
<div class= "proj-container">
    <div class="proj-img" :style="{backgroundImage: imgUrl}"></div>
    <div class="proj-text">
        <h1 class="proj-title">{{title}}</h1>
        <h2 class="proj-org">{{org}}</h2>
        <p class="proj-desc">{{desc}}</p>
    </div>
</div>
</template>

<script>

export default {
    props: {
        imgUrl: String,
        title: String,
        org: String,
        desc: String
    }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Rubik:wght@500&display=swap');
@import url('https://fonts.googleapis.com/css?family=Noto+Sans&display=swap');

.proj-container{
width: 367px;
height: 399.94px;

}

.proj-text{
    background-color: white;
    height: 202px;
border-radius: 0px 0px 28.46px 28.46px;
}
.proj-img{
    height: 250px
}
.proj-title{
    font-family: 'Rubik', sans-serif;
    color:#1A2859;
    font-weight: 100;
    font-size: 24px;
    padding-top: 23px;
}
.proj-org{
    color:#0A2999;
  font-family: 'Noto Sans', sans-serif;
    font-size: 18px;
    padding-top: 7px;
}

.proj-desc{
    padding-top: 7px;
    font-size: 12px;
}

.proj-title, .proj-org, .proj-desc{
    padding-left: 23px;
}
</style>