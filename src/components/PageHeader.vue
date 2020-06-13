<template>
    <header>
        <div class="branding">
            <h1 class="branding__text">
                <span class="branding__text__name">Nick Frost</span>
                <span>Web Developer</span>
            </h1>
        </div>
    </header>
</template>

<style lang="scss">
    $primary: #003da5;

    header {
        background-color: $primary;
        color: white;
        padding: 1.5rem;
    }

    .branding {
        display: flex;

        &__text {
            display: flex;
            flex-direction: column;

            &__name {
                font-weight: bold;
                font-size: 125%;
                margin-bottom: 0.125rem;
            }
        }
    }
</style>