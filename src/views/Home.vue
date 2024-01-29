<template lang="pug">
section#app.section
  form
    h1.title.is-1 {{form.formName}}
    .field
      label.label Alter
      .control
        input.input(type='number', v-model='form.age')
    .field
      label.label Magst du Zwiebelbrot
      .control
        label
          input(type='radio', value='1', v-model='form.zbvotum')
          |  Ja
        br
        label
          input(type='radio', value='0', v-model='form.zbvotum')
          |  Nein
    input.button.is-primary.margin-bottom(type='submit', @click.prevent='fakeSubmit')
  transition(name='fade', mode='out-in')
    article.message.is-primary(v-show='showSubmitFeedback')
      .message-header
        p Fake Send Status:
      .message-body
        | Successfully Submitted!
</template>

<script>
export default {
  name: 'home',
};
</script>