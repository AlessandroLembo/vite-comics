<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            sections: [
                {
                    text: 'Characters',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Comics',
                    url: '#',
                    current: true,
                },
                {
                    text: 'Movies',
                    url: '#',
                    current: false,
                },
                {
                    text: 'TV',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Games',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Collectibles',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Videos',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Fans',
                    url: '#',
                    current: false,
                },
                {
                    text: 'News',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Shop',
                    url: '#',
                    current: false,
                },
            ]

        }
    }

}
</script>

<template>
    <header>
        <div class="container">
            <div class="header-container">
                <figure>
                    <img src="../assets/img/dc-logo.png" alt="logo">
                </figure>
                <nav>
                    <ul class="nav-header">
                        <li v-for="section in sections" class="pdg-sm-space" :class="{ 'active': section.current }"
                            :key="section.text">
                            <a :href="section.url" :class="{ 'active': section.current }"> {{ section.text }} </a>
                        </li>
                    </ul>
                </nav>
            </div>
        </div>

    </header>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/mixins' as *;
@use '../assets/scss/partials/variables' as *;

/* HEADER */
header {
    height: 120px;
    background-color: whitesmoke;
}

.header-container {
    height: $h100;
    @include vertical_algnm;
    justify-content: space-between;

    img {
        cursor: pointer;
    }
}

/* Navbar Header */
nav {
    height: $h100;
}

.nav-header {
    @include vertical_algnm;
    height: $h100;

    a {
        color: black;
        font-weight: 400;
        font-size: 20px;

        &.active {
            color: $dodger;
        }
    }

    li {
        height: $h100;
        @include vertical_algnm;

        &.active {
            border-bottom: 4px solid $dodger;
            padding-top: 4px;
        }
    }

}

/* Utils */
.pdg-sm-space {
    padding: 0 10px;
}
</style>