<template>
    <p>You have {{ numberOfTasks }} tasks!</p>
</template>

<script>
export default {
    computed: {
        numberOfTasks() {
            return this.$store.state.tasks.length;
        }
    }
};
</script>