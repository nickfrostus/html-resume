<template>
    <div>
        <h3>{{ company }}</h3>
        <div class="job-title">{{ job }}</div>
        <ul>
            <li v-for="(responsibility, index) in responsibilities" :key="index">
                » {{ responsibility }}
            </li>
        </ul>
    </div>
</template>

<script>
    export default {
        props: {
            company: String,
            job: String,
            startDate: String,
            endDate: String,
            responsibilities: Array
        }
    }
</script>

<style lang="scss">
    .job-title {
        display: flex;
        margin-top: 0.25rem;
        font-weight: normal;
    }

    ul {
        margin-top: 0.5rem;
        font-size: 87.5%;

        li {
            margin-top: 0.25rem;
        }
    }
</style>