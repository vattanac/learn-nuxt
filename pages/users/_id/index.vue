<template>
    <h1>A single user , with userID: {{ this.$route.params.id }}</h1>
</template>

<script>
    export default {
        validate(data) {
            return /^\d+$/.test(data.params.id)
        }
    }
</script>