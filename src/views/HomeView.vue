<template>
  <div class="content">
    <hr class="min">

    <div class="profile">
      <div class="pic-container">
        <img src="@/assets/images/hika.png" alt="">
      </div>
    </div>
    <h2 class="my-name">
      <strong>HIKA</strong>
    </h2>
    <hr class="min">
    <hr class="full">
    <p class="intro-line">
      I EDIT YOUR VIDEOS WITH PROFICIENCY USING PREMIER PRO AND AFTER EFFECTS WITH HUNDREDS OF HOURS OF EXPERIENCE IN IMPROVING THE WORK QUALITY, PACING, VISUALS, AND LIFESTYLE. TARGETS BOTH VLOGS AND SHORT VIDEOS.
    </p>
    <hr class="full">
    <div class="show-section">
      <div class="wrapper">
        <div class="inner">
          <h2 class="title"><strong>Show Reel 2023</strong></h2>
          <div class="video-container">
            <iframe class="video" src="https://www.youtube.com/embed/ZMQigO6KwQk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
          </div>
        </div>
      </div>
    </div>
    <hr class="min">
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'HomeView',
}
</script>

<style lang="scss" scoped>

.profile {
  &:not(:first-child) {
    margin-top: 1.875rem !important;
  }
  &:not(:last-child) {
    margin-bottom: 1.875rem !important;
  }
  .pic-container {
    border-radius: 100%;
    transition: none;
    text-align: center;
    img {
      transition: none;
    }
  } 
}

.my-name {
  text-transform: uppercase;
  color: #FFFFFF;
  font-family: 'Source Sans Pro', sans-serif;
  letter-spacing: 0.4rem;
  width: calc(100% + 0.4rem);
  font-size: 1.5em;
  line-height: 1.25;
  font-weight: 400;
  text-align: center;
}

.intro-line {
  text-transform: uppercase;
  color: #FFFFFF;
  font-family: 'Source Sans Pro', sans-serif;
  letter-spacing: 0.125rem;
  width: calc(100% + 0.125rem);
  font-size: 0.875em;
  line-height: 1.25;
  font-weight: 400;
  text-align: center;
}

.show-section {
  display: flex;
  width: 100%;
  align-items: center;
  justify-content: center;
  background-color: #703FFC;
  background-size: 256px, cover;
  background-position: center, 0% 0%;
  background-repeat: repeat, repeat;
  border-radius: 0 !important;
  max-width: 100vw;
  position: relative;
  width: 100vw;
  left: 50%;
  margin-left: -50vw;
  right: auto;
  .wrapper {
    max-width: 37rem;
    width: 100%;
    .inner {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      padding: 2rem;
    }
  }
  .title {
    text-transform: uppercase;
    color: #FFFFFF;
    font-family: 'Source Sans Pro', sans-serif;
    letter-spacing: 0.4rem;
    width: calc(100% + 0.4rem);
    font-size: 1.5em;
    line-height: 1.25;
    font-weight: 400;
    text-align: center;
    margin: 0;
  }
  .video-container {
    position: relative;
    overflow: hidden;
    width: 100%;
    padding-top: 56.25%; /* 16:9 Aspect Ratio (divide 9 by 16 = 0.5625) */
    .video {
      position: absolute;
      top: 0;
      left: 0;
      bottom: 0;
      right: 0;
      width: 100%;
      height: 100%;
    }
   
  }
}
@media (max-width: 360px) {
  .my-name {
      font-size: 1.5em;
  }
  .intro-line {
      font-size: 0.875em;
  }
  .show-reel {
      font-size: 1.5em;
  }
  
}

@media (max-width: 480px) {
  .my-name {
      font-size: 1.5em;
  }
}

@media (max-width: 736px) {
  .profile:not(:first-child) {
      margin-top: 1.40625rem !important;
  }
  .profile:not(:last-child) {
      margin-bottom: 1.40625rem !important;
  }
  .profile .pic-container {
      text-align: center;
  }
  
  .my-name {
       letter-spacing: 0.35rem;
       width: calc(100% + 0.35rem);
       font-size: 1.5em;
       line-height: 1.25;
   }
   .intro-line {
    letter-spacing: 0.109375rem;
    width: calc(100% + 0.109375rem);
    font-size: 0.875em;
    line-height: 1.25;
}
.show-reel {
       letter-spacing: 0.35rem;
       width: calc(100% + 0.35rem);
       font-size: 1.5em;
       line-height: 1.25;
   }
}



</style>
