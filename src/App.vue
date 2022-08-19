<template>
  <div id="app">
    <toast-notification></toast-notification>
    <delete-button></delete-button>
  <post-button></post-button>
  </div>
</template>

<script>
import DeleteButton from '@/components/deleteButton.vue';
import ToastNotification from '@/components/toastNotification.vue';
import PostButton from "@/components/postButton.vue";
export default {
  name: 'App',
  components: {
    ToastNotification,
    DeleteButton,
    PostButton
  }
}
</script>

<style>

</style>
