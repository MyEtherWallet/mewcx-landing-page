<template>
  <div>
    <div class="wrapper">
      <div class="header-container pt-4">
        <div class="img-container pt-5"> 
          <img class="mew-logo" alt="Mew logo" src="@/assets/images/logo.png">
        </div>
        <p class="header-text">Browse the blockchain. Bring your own MEW.</p>
        <b-button @click="goToLink()" class="mew-cx-btn">Download MEW CX
          <img class="ml-3 arrow" src="@/assets/images/arrow-2.png"/>
        </b-button>
      </div>
      <img class="mew-site" alt="mew-site" src="@/assets/images/image.png">
      <img class="footer-design" alt="footer-design" src="@/assets/images/2.png">
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    goToLink() {
      window.open('https://chrome.google.com/webstore/detail/myetherwallet-extension/nlbmnnijcnlegkjjpcfjclmcfggfefdm?hl=en')
    }
  }
}
</script>

<style lang="scss" scoped>
@import 'Header.scss';
</style>