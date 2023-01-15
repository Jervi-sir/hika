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
        discord id :- <u id="discord"  @click="copyMe('discord', discord)">{{ discord }}</u>
        <br>
        email :- <u id="email" @click="copyMe('email', email)">{{ email }}</u>
      </span>
    </p>
    <div class="credit">
      © 2023 Hika. All Rights Reserved.
    </div>
    <hr class="min">
    <hr class="full">
    <transition>
      <div v-if="showAnnotation" id="copied" v-bind:style="{ top: (mousePosX-100) + 'px', left: (mousePosY+100) + 'px'}">
        <span>{{ type }} link</span>
        <span>copied</span>
      </div>
    </transition>
  </div>
  
</template>

<script>


export default {
  data () {
    return {
      discord: 'Hika#2704',
      email: 'imhika1@gmail.com',
      type: '',
      showAnnotation: false,
    }
  },
  methods: {
    copyMe (type, text) { 
      //var X = this.mousePosX;
      //var Y = this.mousePosY;
      //console.log(X, Y);
      this.showAnnotation = true;
      navigator.clipboard.writeText(text);
      this.type = type;
      setTimeout(() => this.showAnnotation = false, 1000);

    },
  },

  mounted() {
    //document.addEventListener("mousemove", (event) => {
      //this.mousePosX = event.clientX;
      //this.mousePosY = event.clientY;
    //});
  },
  name: 'ContactView',
  
}
</script>

<style lang="scss" scoped>
.v-enter-active,
.v-leave-active {
  transition: opacity 0.3s ease;
}

.v-enter-from,
.v-leave-to {
  opacity: 0;
}
#copied {
  position: absolute;
  top:50%;
  left:50%;
  transform: translate(-50%, -50%);
  color: black;
  background: white;
  padding: 2px 6px;
  border-radius: 1rem;
  font-size: 12px;
  text-align: center;
  width: 100px;
  height: 100px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  font-weight: 600;
  font-size: 15px;
}

.scale {
  transform: scale(1.1125);
}
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

u:hover {
  cursor: pointer;
  color: #542CF2;
  transition: 0.3s;
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