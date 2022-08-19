<template>
    <div>
        <button @click="send_message" >Delete</button>
    </div>
</template>

<script>
    export default {
        methods: {
            send_message() { 
                this.$root.$emit(`toast_notify`, `success delete`);
            },
        },
        
    }
</script>

<style scoped>

</style>