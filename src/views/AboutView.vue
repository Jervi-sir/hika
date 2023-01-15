<template>
  <div class="about">
    <hr class="min">
    <h1 class="title">About Me</h1>
    <p class="description">
      <span class="text">
      Hey my name is hika and im Helping creators get to their dream goals creating the best content possible .I believe that attention is the new currency and my goal is to be a way for all creators to tap into this new currency and help them build good forever improving content which people love and enjoy! Videos with high viewer retention scores tend to go viral. On YouTube, a higher score means increased visibility on YouTube’s platform. Viewers retain 95% of a message when they watch it in a video compared to 10% when reading it in text. 
      <br>
      Interested? 
      </span>
      <br>
      <a class="get-in-touch" @click="$router.push('/contact')">Get in touch</a>!
      
    </p>
    <hr class="min">
    <hr class="full">
  </div>
</template>

<script>

export default {
  created () {
  },
  name: 'AboutView',
  
}
</script>

<style lang="scss" scoped>
.title {
  text-transform: uppercase;
  color: #FFFFFF;
  font-family: 'Source Sans Pro', sans-serif;
  letter-spacing: 0.175rem;
  width: calc(100% + 0.175rem);
  font-size: 1em;
  line-height: 1.375;
  font-weight: 700;
  text-align: center;
}

.description {
  color: #FFFFFF;
  font-family: 'Source Sans Pro', sans-serif;
  letter-spacing: 0.025rem;
  width: calc(100% + 0.025rem);
  font-size: 1em;
  line-height: 1.875;
  font-weight: 400;
  text-align: center;
  overflow-wrap: break-word;

  .text {
    margin-top: 1rem;
  }
  .get-in-touch {
    cursor: pointer;
    text-decoration: underline;
    color: #FFFFFF;
    text-align: center;
    &:hover {
      color: #309EDB;
      transition: 0.2s;
    }
  }
}

@media (max-width: 736px) {
  .description {
    letter-spacing: 0.021875rem;
    font-size: 1em;
    line-height: 1.875;
    width: 90%;
    margin:auto;

  }
}
@media (max-width: 360px) {
  .description {
        font-size: 1em;
  }
}
</style>