<template>
    <div>
        <h3>{{ title }}</h3>
        <ul>
            <li v-for="(skill, index) in skills" :key="index">
                » {{ skill }}
            </li>
        </ul>
    </div>
</template>

<script>
    export default {
        props: {
            title: String,
            skills: Array
        }
    }
</script>