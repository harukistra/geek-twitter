<template>
    <div class="form__wrapper">
      <textarea 
      class="form__textarea"
      v-model="text"
      placeholder="What are u doing now??"
      />
      <div class="form__buttons">
        <button v-on:click="postTweet" class="form__submit-button">
        post</button>
      </div>
    </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'

export default {
  data() {
    return {
      text: "",
    }
  },
  methods: {
    postTweet() {
      alert("you're ganna be excited to see the competed posting function!!")
    },
  },
}
</script>

<style scoped>
.form__wrapper {
  padding: 1rem;
}
.form__textarea {
  width: 100%;
  height: calc(1.3rem * 3 + 0.5rem * 2);
  padding: 0.5rem;
  line-height: 1.3rem;
  border-radius: 5px;
  border: none;
  resize: none;

}
.form__textarea:focue {
  outline: none;
}
.form_buttons {
  display: flex;
  justify-content: flex-end;
}

</style>