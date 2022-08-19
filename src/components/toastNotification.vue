<template>
<div>
<div v-if="notification !== undefined">
    <h2>{{notification}}</h2>
    <button @click="dismiss_notify" >Dismiss</button>
</div>

</div>
</template>

<script>
    export default {
        methods: {
            show_message(message) {
                this.notification = message;
            },
              dismiss_notify(){
            this.notification = undefined;
        },
        },
      
        mounted () {
            this.$root.$on(`toast_notify`,this.show_message);
        },
        data() {
            return {
                notification: undefined
            }
        },
    }
</script>

<style scoped>

</style>