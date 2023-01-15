<template>
  <div class="social-links">
    <a href="" class="social"><img src="@/assets/images/twitter.svg" alt=""></a>
    <a href="" class="social"><img src="@/assets/images/discord.svg" alt=""></a>
    <a href="" class="social"><img src="@/assets/images/email.svg" alt=""></a>
    <a href="" class="social"><img src="@/assets/images/instagram.svg" alt=""></a>
  </div>
</template>

<script>
export default {
  watch: {
  },
  methods: {
  },
  name: 'SocialMedia',
}
</script>

<style lang="scss" scoped>
.social-links {
  display: flex;
  justify-self: center;
  justify-content: center;
  gap: 1.125rem;
  .social {
    padding: 12px;
    background: #5C32F5;
    background-image: linear-gradient(84deg, #703FFC 0%, rgba(84,44,242,0.008) 100%);
    background-position: 0% 0%;
    background-repeat: repeat;
    background-size: cover;
    box-shadow: 0rem 0rem 0.375rem 0rem #080202;
    border-radius: 100%;
    transition: transform 0.25s ease, color 0.25s ease, background-color 0.25s ease, border-color 0.25s ease;
    align-items: center;
    display: flex;
    justify-content: center;
    img {
      color: #FFFFFF;
      height: 30px;
      width: 30px;
    }

    &:hover {
      background-color: #309EDB !important;
      transform: scale(1.1125);
    }
  }
}
</style>


