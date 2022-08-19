<template>
  <footer class="py-5">
    <v-container>
      <v-row>
        <v-col cols="12" md="4" class="d-flex justify-center justify-md-start">
          <a href="mailto:support@myetherwallet.com" class="white--text">Support</a>
          <a href="https://www.myetherwallet.com/privacy-policy" class="white--text mx-8">Privacy</a>
          <a href="https://www.myetherwallet.com/terms-of-service" class="white--text">Terms</a>
        </v-col>
        <v-col cols="12" md="4" class="teal--text text-center">
          © 2022 MyEtherWallet. All rights reserved.
        </v-col>
        <v-col cols="12" md="4" class="d-flex justify-center justify-md-end">
          <a
            v-for="link in links"
            :key="link.class"
            :href="link.to"
            target="_blank"
            class="mx-1 d-flex align-center"
          >
            <v-icon v-if="link.icon" size="17px" class="teal--text">
              {{ link.icon }}
            </v-icon>
            <img v-else height="17" :src="link.img" alt="icon" />
          </a>
        </v-col>
      </v-row>
    </v-container>
  </footer>
</template>

<script>
import Medium from '@/assets/img/medium.svg';
export default {
  name: 'FooterBlock',
  data: () => ({
    links: [
      {
        to: 'https://www.facebook.com/myetherwallet',
        icon: 'mdi-facebook'
      },
      {
        to: 'https://www.twitter.com/@myetherwallet',
        icon: 'mdi-twitter'
      },
      {
        to: 'https://www.instagram.com/myetherwallet',
        icon: 'mdi-instagram'
      },
      {
        to: 'https://www.linkedin.com/company/myetherwallet',
        icon: 'mdi-linkedin'
      },
      {
        to: 'https://www.github.com/myetherwallet',
        icon: 'mdi-github'
      },
      {
        to: 'https://www.reddit.com/r/myetherwallet',
        icon: 'mdi-reddit'
      },
      {
        to: 'https://www.medium.com/@myetherwallet',
        img: Medium
      },
      {
        to: 'https://vk.com/public190491855',
        icon: 'mdi-vk'
      },
      {
        to: 'https://t.me/myetherwallet',
        icon: 'mdi-telegram'
      }
    ]
  })
};
</script>

<style lang="scss" scoped>
* {
  font-size: 14px;
  font-weight: 500;
}
.white--text {
  color: white;
}
.black--text {
  color: black;
}
.teal--text {
  color: #96a8b6;
}
.text-transform--none {
  text-transform: none;
}
a {
  cursor: pointer;
  text-decoration: none;
}
footer {
  background-color: #13273e;
}
</style>
