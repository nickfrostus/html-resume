<template>
  <div id="app">
    <page-header/>

    <h2>Experience</h2>
    <div class="container container--experience">
      <experience company="Hippo Manager Software, Inc."
                  job="Lead Software Engineer"
                  start-date="2022"
                  end-date="Present"
                  :responsibilities="[
                        'Managed infrastructure and other administrative level tasks.',
                        'Saved the company in excess of $6,000 monthly in AWS.',
                        'Made product direction decisions with team.',
                        'Worked directly with clients to get feature feedback.'
                    ]"/>
      <experience company="Kalamazoo Valley Community College"
                  job="Senior Web Developer"
                  start-date="2017"
                  end-date="2022"
                  :responsibilities="[
                        'Wrote and maintained web applications from scratch.',
                        'Defined CI/CD workflow with Github Actions/Docker.',
                        'Provisioned and defined web infrastructure.',
                        'Lead project meetings for feature requirements.'
                    ]"/>
    </div>

    <h2>Notable Projects</h2>
    <div class="container">
      <notable-project title="Hippo Manager 2.0"
                       client="Hippo Manager Software, Inc."
                       technologies="Vue.js, Laravel, SASS/SCSS, Tailwind CSS"
                       description="Hippo Manager is a full suite of software for managing veterinary clinics/practices. This cloud-based software does everything you need to manage a veterinary business, billing, client management, scheduling, etc."
                       link="https://www.nfrost.dev/hippo-manager"/>
      <notable-project title="Course Schedule"
                       client="Kalamazoo Valley Community College"
                       technologies="Vue.js, .NET, SASS/SCSS, Tailwind CSS"
                       description="The Kalamazoo Valley Course Schedule is an application that displays for-credit courses offered at Kalamazoo Valley Community College; and allows users to filter results based on relevant criteria."
                       link="https://www.nfrost.dev/kvcc-course-schedule"/>
    </div>

    <h2>Skill Set</h2>
    <div class="container container--skillset">
      <skill-set title="Languages"
                 :skills="['JavaScript', 'C#', 'PHP', 'Golang', 'HTML', 'SCSS/SASS/CSS', 'SQL & GraphQL',]"/>
      <skill-set title="Frameworks"
                 :skills="['Laravel/Lumen', '.NET', 'Vue/Nuxt', 'Hugo', 'Svelte', 'React']"/>
      <skill-set title="Infrastructure"
                 :skills="['Docker', 'Github Actions', 'Nginx', 'Apache', 'Firebase', 'Google Cloud Platform', 'Amazon Web Services']"/>
      <skill-set title="CMS"
                 :skills="['Prismic', 'Cockpit', 'WordPress', 'Drupal']"/>
      <skill-set title="Data Analysis"
                 :skills="['Google Analytics', 'SEO', 'Database Normalization', 'Design Documentation']"/>
      <skill-set title="Applications"
                 :skills="['JetBrains IDEs', 'Adobe Photoshop', 'Adobe Illustrator', 'Microsoft Office', 'Figma']"/>
      <skill-set title="Dependencies"
                 :skills="['Git Submodules', 'Composer', 'NuGet', 'NPM']"/>
      <skill-set title="Platforms"
                 :skills="['Github', 'Basecamp', 'Trello', 'Sentry', 'Jira']"/>
    </div>

    <h2>Education</h2>
    <div class="container">
      <education title="Visual Communications"
                 type="Associate of Applied Science"
                 institution="ITT Technical Institute"/>
      <education title="Vue JS 2 - The Complete Guide"
                 type="Online Course"
                 institution="Udemy"/>
    </div>
  </div>
</template>

<script>
import PageHeader from './components/PageHeader'
import Experience from "./components/Experience";
import NotableProject from "./components/NotableProject";
import SkillSet from "./components/SkillSet";
import Education from "./components/Education";

export default {
  components: {PageHeader, Education, SkillSet, NotableProject, Experience}
}
</script>

<style lang="scss">
$primary: #003da5;

#app {
  width: 8.5in;
  height: 11in;
  font-family: "Titillium Web", sans-serif;
  background-color: white;
  font-weight: 300;
  display: flex;
  flex-direction: column;
}

h2 {
  font-size: 150%;
  color: $primary;
  font-weight: bold;
  padding: 1.5rem 1.5rem 1rem;
  border-top: 0.0625rem solid $primary;
}

h3 {
  font-weight: 600;
  font-size: 125%;
}

ul {
  margin-top: 0.5rem;
  font-size: 87.5%;

  li {
    margin-top: 0.25rem;
  }
}

.container {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-gap: 1.5rem;
  padding: 0 1.5rem 1.5rem;

  &--skillset {
    grid-template-columns: repeat(4, 1fr);
  }
}
</style>
