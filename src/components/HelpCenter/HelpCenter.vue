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
        :question="'Balances not loading or showing on MyEtherWallet'"
        :answer="'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Idcirco enim non desideraret, quia, quod dolore caret, id in voluptate est. Nihil ad rem! Ne sit sane; Nam, ut saepe iam dixi, in infirma aetate inbecillaque mente vis naturae quasi per caliginem cernitur'"
      ></qa-toggle>
      <qa-toggle
        :question="'Does MyEtherWallet support Bitcoin or other coins (LTC STEEM ZEC)?'"
        :answer="'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Idcirco enim non desideraret, quia, quod dolore caret, id in voluptate est. Nihil ad rem! Ne sit sane; Nam, ut saepe iam dixi, in infirma aetate inbecillaque mente vis naturae quasi per caliginem cernitur'"      
      ></qa-toggle>
      <qa-toggle
        :question="'ETH or tokens sent to or from exchange haven\'t shown up'"
        :answer="'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Idcirco enim non desideraret, quia, quod dolore caret, id in voluptate est. Nihil ad rem! Ne sit sane; Nam, ut saepe iam dixi, in infirma aetate inbecillaque mente vis naturae quasi per caliginem cernitur'"
      ></qa-toggle>
      <qa-toggle
        :question="'Where can I buy / sell / trade / exchange my ETH or tokens?'"
        :answer="'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Idcirco enim non desideraret, quia, quod dolore caret, id in voluptate est. Nihil ad rem! Ne sit sane; Nam, ut saepe iam dixi, in infirma aetate inbecillaque mente vis naturae quasi per caliginem cernitur'"
      ></qa-toggle>
      <qa-toggle
        :question="'What is an ICO?'"
        :answer="'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Idcirco enim non desideraret, quia, quod dolore caret, id in voluptate est. Nihil ad rem! Ne sit sane; Nam, ut saepe iam dixi, in infirma aetate inbecillaque mente vis naturae quasi per caliginem cernitur'"
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