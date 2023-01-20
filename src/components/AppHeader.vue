<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            links: [
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
                        <li class="pdg-sm-space"><a href="#">Characters</a></li>
                        <li class="pdg-sm-space active"><a class="active" href="#">Characters</a></li>
                        <li class="pdg-sm-space"><a href="#">Characters</a></li>
                        <li class="pdg-sm-space"><a href="#">Characters</a></li>
                        <li class="pdg-sm-space"><a href="#">Characters</a></li>
                        <li class="pdg-sm-space"><a href="#">Characters</a></li>
                        <li class="pdg-sm-space"><a href="#">Characters</a></li>
                        <li class="pdg-sm-space"><a href="#">Characters</a></li>
                        <li class="pdg-sm-space"><a href="#">Characters</a></li>
                        <li class="pdg-sm-space"><a href="#">Characters</a></li>

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
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
}

.header-container {
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

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

.nav-header a {
    color: black;
}

.nav-header a.active {
    color: dodgerblue;
}

/* Utils */
.pdg-sm-space {
    padding: 0 10px;
}
</style>