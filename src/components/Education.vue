<template>
    <div>
        <h3>{{ title }}</h3>
        <div class="type">{{ type }}</div>
        <div class="institution">{{ institution }}</div>
    </div>
</template>

<script>
    export default {
        props: {
            title: String,
            type: String,
            institution: String
        }
    }
</script>

<style lang="scss">
    .type {
        margin-top: 0.125rem;
    }

    .institution {
        font-style: italic;
        margin-top: 0.25rem;
        font-size: 87.5%;
    }
</style>