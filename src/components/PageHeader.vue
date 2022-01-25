<template>
    <header>
        <div class="branding">
            <svg viewBox="0 0 78 48" fill="none" xmlns="http://www.w3.org/2000/svg" class="logo">
                <path d="M0 38.9943V48H20.9161H29.8866V17.9962L47.8277 48H56.7982V28.4952H71.7339V19.5048H56.7982V9.00571H77.7143V0H56.7982H47.8277V30.0038L29.8866 0H20.9161V19.5048H5.98036V28.4952H20.9161V38.9943H0Z"></path>
            </svg>
            <h1 class="branding__text">
                <span class="branding__text__name">Nick Frost</span>
                <span>Web Developer</span>
            </h1>
        </div>
        <nav class="nav">
            <a href="https://www.nfrost.dev/" class="nav__link">
                <font-awesome-icon icon="globe-americas" class="nav__link__icon"/>
                <span>www.nfrost.dev</span>
            </a>
            <a href="mailto:nfrost.dev@gmail.com" class="nav__link">
                <font-awesome-icon :icon="['far', 'envelope']" class="nav__link__icon"/>
                <span>nfrost.dev@gmail.com</span>
            </a>
            <a href="https://github.com/nfrostdev" class="nav__link">
                <font-awesome-icon :icon="['fab', 'github']" class="nav__link__icon"/>
                <span>github.com/nfrostdev</span>
            </a>
        </nav>
    </header>
</template>

<style lang="scss">
    $primary: #003da5;

    header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        background-color: $primary;
        color: white;
        padding: 1.5rem;
    }

    .branding {
        display: flex;
        line-height: 100%;

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

    .logo {
        width: 3.25rem;
        fill: white;
        margin-right: 0.5rem;
    }

    .nav {
        display: flex;

        &__link {
            display: flex;
            justify-content: center;
            align-items: center;
            color: white;
            text-decoration: none;
            margin: 0 1rem;

            &__icon {
                margin-right: 0.25rem;
            }
        }
    }
</style>