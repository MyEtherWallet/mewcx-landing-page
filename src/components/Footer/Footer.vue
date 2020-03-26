<template>
  <div>
    <b-container>
        <b-row class="wrapper">
          <div class="support-links">
            <a href="mailto:support@myetherwallet.com" target="_blank">Support</a>
            <a href="https://www.myetherwallet.com/privacy-policy">Privacy</a>
            <a href="https://www.myetherwallet.com/terms-and-conditions">Terms</a>
          </div>
          <div class="copyright-txt mt-1">© 2020 MyEtherWallet. All rights reserved. </div>
          <div class="social-links">
              <a
                v-for="link in links"
                :key="link.class"
                :href="link.to"
                :aria-label="link.to"
                rel="noopener noreferrer"
                target="_blank"
              >
                <i :class="'fa ' + link.class" />
              </a>
          </div>
        </b-row>
    </b-container>
  </div>
</template>

<script>
export default {
  data() {
    return {
      links: [
        {
          to: 'https://www.facebook.com/myetherwallet',
          class: 'fa-facebook'
        },
        {
          to: 'https://www.twitter.com/@myetherwallet',
          class: 'fa-twitter'
        },
        {
          to: 'https://www.instagram.com/myetherwallet',
          class: 'fa-instagram'
        },
        {
          to: 'https://www.linkedin.com/company/myetherwallet',
          class: 'fa-linkedin'
        },
        {
          to: 'https://www.github.com/myetherwallet',
          class: 'fa-github'
        },
        {
          to: 'https://www.reddit.com/r/myetherwallet',
          class: 'fa-reddit-alien'
        },
        {
          to: 'https://www.medium.com/@myetherwallet',
          class: 'fa-medium'
        },
        {
          to: 'https://vk.com/public190491855',
          class: 'fa-vk'
        },
        {
          to: 'https://t.me/myetherwalletofficial',
          class: 'fa-telegram'
        }
      ]
    };
  }
}
</script>

<style lang="scss" scoped>
@import 'Footer.scss';
</style>
