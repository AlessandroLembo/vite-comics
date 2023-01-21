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
                        <li v-for="section in sections" class="pdg-sm-space" :class="{ 'active': section.current }">
                            <a :href="section.url" :class="{ 'active': section.current }"> {{ section.text }} </a>
                        </li>
                    </ul>
                </nav>
            </div>
        </div>

    </header>
</template>

<style scoped>
/* HEADER */
header {
    height: 120px;
}

.header-container {
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.header-container img {
    cursor: pointer;
}

/* Navbar Header */
nav {
    height: 100%;
}

.nav-header {
    display: flex;
    align-items: center;
    height: 100%;
}

.nav-header li {
    height: 100%;
    display: flex;
    align-items: center;
}

.nav-header li.active {
    border-bottom: 4px solid dodgerblue;
    padding-top: 4px;
}

/* Utils */
.pdg-sm-space {
    padding: 0 10px;
}

.nav-header a {
    color: black;
    font-weight: 400;
    font-size: 20px;
}

.nav-header a.active {
    color: dodgerblue;
}
</style>