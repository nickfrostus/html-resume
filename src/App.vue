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
    </div>
</template>

<script>
    import Experience from "./components/Experience";

    export default {
        components: {Experience}
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
    }
</style>
