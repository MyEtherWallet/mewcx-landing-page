<template>
  <div class="faq-wrapper">
    <div class="header-container">
      <span class="header">FAQs</span>
      <div>
        <a class="help-link" href="https://kb.myetherwallet.com/">Help Center</a>
        <a href="mailto:support@myetherwallet.com" target="_blank">Contact Support</a>
      </div>
    </div>
    <div class="body-container">
      <hr align="center">
      <qa-toggle
        :question="'MyEtherWallet: An Introduction'"
        :answer="'https://kb.myetherwallet.com/en/getting-started/myetherwallet-an-introduction/'"
      ></qa-toggle>
      <qa-toggle
        :question="'What’s the Difference Between an Exchange (i.e. Coinbase, Kraken, Gemini, Binance, etc.) and MyEtherWallet?'"
        :answer="'https://kb.myetherwallet.com/en/getting-started/difference-between-mew-and-exchange/'"      
      ></qa-toggle>
      <qa-toggle
        :question="'How to Create a Wallet'"
        :answer="'https://kb.myetherwallet.com/en/getting-started/how-to-create-a-wallet/'"
      ></qa-toggle>
    </div>
  </div>
</template>

<script>
import QAToggle from '../QAToggle';

export default {
  components: {
  'qa-toggle': QAToggle
  },
}
</script>

<style lang="scss" scoped>
@import 'HelpCenter.scss';
</style>