<template>
  <div class="contact">
    <hr class="min">
    <h1 class="title">Contact</h1>
    <p class="contact-list">
      <span class="p">
        Mail Me A Proposal To Get A FREE Sample.
        <br>
        Contact Me Or Network With Me By soclais linked below.
        <br>
        looking forward to hearing from you awesome people!
        <br>
        discord id :- Hika#2704
        <br>
        email :- hika@gmail.com
      </span>
    </p>
    <div class="credit">
      © 2023 Hika. All Rights Reserved.
    </div>
    <hr class="min">
    <hr class="full">
  </div>
</template>

<script>

export default {
  created () {
  },
  name: 'ContactView',
  
}
</script>

<style lang="scss" scoped>
.title {
  text-transform: uppercase;
  color: #FFFFFF;
  letter-spacing: 0.4rem;
  width: calc(100% + 0.4rem);
  font-size: 1em;
  line-height: 1.5;
  font-weight: 700;
  text-align: center;
}
.contact-list {
  color: #FFFFFF;
  letter-spacing: 0.025rem;
  width: calc(100% + 0.025rem);
  font-size: 1em;
  line-height: 1.875;
  font-weight: 400;
  margin-top: 1rem;
  text-align: center;
span {
  &.p:nth-child(n + 2) {
    margin-top: 1rem;
  }
}

}
.credit {
  color: #FFFFFF;
  font-family: 'Source Sans Pro', sans-serif;
  letter-spacing: 0.025rem;
  width: calc(100% + 0.025rem);
  font-size: 1em;
  line-height: 1.875;
  font-weight: 300;
  text-align: center;

}
@media (max-width: 736px) {
  .contact-list {
       letter-spacing: 0.021875rem;
       width: calc(100% + 0.021875rem);
       font-size: 1em;
       line-height: 1.875;
   }
   .credit {
       letter-spacing: 0.021875rem;
       width: calc(100% + 0.021875rem);
       font-size: 1em;
       line-height: 1.875;
   }
}

@media (max-width: 480px) {
  
}

@media (max-width: 360px) {
  .contact-list, .credit {
      font-size: 1em;
  }
}
</style>