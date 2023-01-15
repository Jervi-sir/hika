<template>
  <hr class="full">
  <nav class="menu">
    <router-link class="tab" to="/" ><span>Home</span></router-link>
    <router-link class="tab" to="/work" ><span>Work</span></router-link>
    <router-link class="tab" to="/contact" ><span>Contact</span></router-link>
    <router-link class="tab" to="/about" ><span>About Me</span></router-link>
  </nav>
  <hr class="full">
  <router-view/>
  <SocialMedia />

</template>
<script>
import SocialMedia from '@/components/SocialMedia.vue'
export default {
  components: {
    SocialMedia
  }
}
</script>


<style lang="scss" scoped>
  .menu {
    gap: 0.5rem;
    flex-direction: row;
    flex-wrap: wrap;
    display: flex;
    justify-content: center;
    &:not(:first-child) {
      margin-top: 1.375rem !important;
    }
    &:not(:last-child) {
      margin-bottom: 1.375rem !important;
    }
    span {
      color: #FFFFFF;
      border: solid 1px #FFFFFF;
    }
    span:hover {
      border-color: #309EDB !important;
      color: #309EDB !important;
    }
    .tab {
      
      span {
        display: inline-block;
        width: 6.5rem;
        height: 2.25rem;
        line-height: calc(2.25rem - 2px);
        padding: 0 0.5rem;
        vertical-align: middle;
        text-transform: uppercase;
        font-family: 'Source Sans Pro', sans-serif;
        letter-spacing: 0.225rem;
        padding-left: calc(0.225rem + 0.5rem);
        font-size: 0.625em;
        font-weight: 400;
        border-radius: 1.625rem;
        direction: var(--site-language-direction);
        overflow: hidden;
        text-overflow: ellipsis;
        transition: color 0.25s ease, background-color 0.25s ease, border-color 0.25s ease;
        text-align: center;
      }
      &.active  {
        span {
          border-color: #309EDB !important;
          color: #309EDB !important;
        }
      }
    }
  }


  @media (max-width: 736px) {
    .menu {
        gap: 0.5rem;
    }
    .menu:not(:first-child) {
        margin-top: 1.03125rem !important;
    }
    .menu:not(:last-child) {
        margin-bottom: 1.03125rem !important;
    }
    .menu .tab span {
      letter-spacing: 0.225rem;
      padding-left: calc(0.225rem + 0.5rem);
      font-size: 0.625em;
    }
  }
  @media (max-width: 480px) {
    .menu .tab span {
       width: 6.5rem;
    }
  }
  @media (max-width: 360px) {
    .menu {
       gap: 0.375rem;
   }
  }



</style>

<style lang="scss">
@import '@/assets/global.scss';
#app {
  --padding-horizontal: 1rem;
    --padding-vertical: 1.25rem;
    --spacing: 1.125rem;
    --width: 37rem;
    border-radius: var(--border-radius-tl) var(--border-radius-tr) var(--border-radius-br) var(--border-radius-bl);
    max-width: 100%;
    position: relative;
    width: var(--width);
    z-index: 1;
}
</style>
