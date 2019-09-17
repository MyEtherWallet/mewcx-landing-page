<template>
  <div>
    <div class="question-container">
      <span class="question-txt">{{question}}</span>
      <span class="toggle-icon" v-show="hideAnswerContainer" @click="hideAnswerContainer = !hideAnswerContainer">+</span>
      <span class="toggle-icon" v-show="!hideAnswerContainer" @click="hideAnswerContainer = !hideAnswerContainer">-</span>
    </div>
    <div v-show="!hideAnswerContainer" class="answer-container">
      <a :href="answer">{{answer}}</a>
    </div>
    <hr align="center">
  </div>
</template>

<script>
export default {
  data() {
    return {
      hideAnswerContainer: true,
    };
  },
  props: {
    question: {
      type: String,
      default: ''
    },
    answer: {
      type: String,
      default: ''
    }
  },
  methods: {
    toggleAnswer() {

    }
  }
}
</script>

<style lang="scss" scoped>
@import 'QAToggle.scss';
</style>