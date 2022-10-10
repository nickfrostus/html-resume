<template>
  <div>
    <h3>{{ title }}</h3>
    <ul>
      <li v-for="(skill, index) in sortedSkills" :key="index">
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
  },
  computed: {
    sortedSkills() {
      return this.skills.sort((a, b) => a > b ? 1 : -1)
    }
  }
}
</script>