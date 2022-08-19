<template>
  <div>
    <v-container class="home--mewcx-enkrypt text-center py-15 px-5">
      <img src="@/assets/img/logo.svg" alt="MEWcx" height="35" />

      <div
        class="block-bold block-title"
        :class="isMobile ? 'mobile my-9' : 'mt-10 mb-11'"
      >
        MEWcx is now Enkrypt
      </div>

      <div class="mb-15">
        <a href="https://www.enkrypt.com/" target="_blank">
          <v-btn
            height="55px"
            class="background-color"
            size="x-large"
            rounded="pill"
          >
            <div
              class="px-3 text-transform--none white--text font-weight-bold"
              :class="isMobile ? 'mew-heading-3' : 'goto-btn'"
            >
              Go to Enkrypt.com
            </div>
          </v-btn>
        </a>
      </div>

      <img
        style="max-width: 800px; width: 100%; border-radius: 30px;"
        src="@/assets/img/interface.jpeg"
        alt="Enkrypt interface"
      />
    </v-container>

    <div class="background-color py-12 px-7 text-center">
      <div
        class="white--text mx-auto banner-text text-center mb-6"
        :class="isMobile ? 'mobile' : ''"
      >
        We've upgraded and improved everything that MEWcx had to offer! Install
        Enkrypt, our multichain browser extension!
      </div>
      <a href="https://www.enkrypt.com/" target="_blank">
        <v-btn size="x-large" rounded="pill">
          <div class="text-transform--none black--text font-weight-bold">
            Go to Enkrypt.com
          </div>
        </v-btn>
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeLanding',
  data: () => ({
    windowWidth: window.innerWidth
  }),
  computed: {
    isMobile() {
      return this.windowWidth < 600;
    }
  },
  mounted() {
    this.$nextTick(() => {
      window.addEventListener('resize', this.onResize);
    });
  },
  beforeUnmount() {
    window.removeEventListener('resize', this.onResize);
  },
  methods: {
    onResize() {
      this.windowWidth = window.innerWidth;
    }
  }
};
</script>

<style lang="scss" scoped>
.block-bold {
  font-weight: 900;
}
.block-title {
  font-size: 48px;
  &.mobile {
    font-size: 36px;
    line-height: 46px;
  }
}
.goto-btn {
  font-size: 24px;
}
.background-color {
  background: linear-gradient(86.81deg, #c549ff -22.41%, #704bff 120.76%);
}
.banner-text {
  font-size: 20px;
  max-width: 600px;
  &.mobile {
    font-size: 16px;
    line-height: 24px;
  }
}
.white--text {
  color: white;
}
.black--text {
  color: black;
}
.text-transform--none {
  text-transform: none;
}
a {
  text-decoration: none;
}
</style>
