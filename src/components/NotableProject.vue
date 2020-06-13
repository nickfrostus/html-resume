<template>
    <div>
        <h3>{{ title }}</h3>
        <div class="client">{{ client }}</div>
        <div class="languages">{{ languages }}</div>
        <p class="description">{{ description }}</p>
        <div class="more-info"><a :href="link">{{ link }}</a></div>
    </div>
</template>

<script>
    export default {
        props: {
            title: String,
            client: String,
            languages: String,
            description: String,
            link: String
        }
    }
</script>

<style lang="scss">
    $primary: #003da5;

    .client, .description {
        margin-top: 0.25rem;
        font-size: 87.5%;
    }

    .languages {
        font-weight: normal;
        margin-top: 0.25rem;
    }

    .description {
        line-height: 125%;
    }

    .more-info {
        margin-top: 0.375rem;
        font-size: 87.5%;
        line-height: 125%;

        a {
            color: $primary;
        }
    }
</style>