<template>
  <div>
 <button @click="post_notify">Post</button>
  </div>
</template>

<script>
export default {
  methods: {
    post_notify() {
      this.$root.$emit(`toast_notify` , `success_post`);
    }
  },

};
</script>

<style scoped></style>
