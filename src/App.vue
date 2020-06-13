<template>
    <div id="app">
        <h2>Experience</h2>
        <div class="container container--experience">
            <experience company="Kalamazoo Valley Community College"
                        job="Web Developer"
                        start-date="2017"
                        end-date="Present"
                        :responsibilities="[
                        'Wrote and maintained web applications from scratch.',
                        'Defined CI/CD workflow with Github Actions.',
                        'Provisioned and defined web infrastructure.',
                        'Lead project meetings for feature requirements.'
                    ]"/>
            <experience company="T-Shirt Printing Plus"
                        job="Sign Department Manager"
                        start-date="2013"
                        end-date="2017"
                        :responsibilities="[
                        'Designed print documents and assessed customer needs.',
                        'Modified pricing according to desired margins quarterly.',
                        'Maintained computers and wide-format printers.',
                        'Ordered materials for projects weekly.'
                    ]"/>
        </div>
        <h2>Notable Projects</h2>
        <div class="container">
            <notable-project title="Employee Directory"
                             client="Kalamazoo Valley Community College"
                             languages="C#, HTML, SCSS, JavaScript, SQL"
                             description="The Kalamazoo Valley Employee Directory is a searchable database of current employees at Kalamazoo Valley Community College. This is one half of a larger project that also includes the Department Directory."
                             link="https://www.nfrost.dev/employee-directory"/>
            <notable-project title="Department Directory"
                             client="Kalamazoo Valley Community College"
                             languages="C#, HTML, SCSS, JavaScript, SQL"
                             description="The Department Directory is the counterpart to the Employee Directory, meant to assist users with finding the correct department pertaining to a specific topic they need information about at Kalamazoo Valley."
                             link="https://www.nfrost.dev/department-directory"/>
        </div>
    </div>
</template>

<script>
    import Experience from "./components/Experience";
    import NotableProject from "./components/NotableProject";

    export default {
        components: {NotableProject, Experience}
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
    }

    h2 {
        font-size: 150%;
        color: $primary;
        font-weight: bold;
        padding: 2rem 2rem 1rem;
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
        grid-gap: 2rem;
        padding: 0 2rem 2rem;
        border-bottom: 0.0625rem solid $primary;
    }
</style>
