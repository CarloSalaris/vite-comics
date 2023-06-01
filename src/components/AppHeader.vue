<script>

export default {
    name: "AppHeader",
    data() {
        return {
            links: [
                {
                    text: 'CHARACTERS',
                    url: '#',
                    current: false,
                }, {
                    text: 'COMICS',
                    url: '#',
                    current: true,
                }, {
                    text: 'MOVIES',
                    url: '#',
                    current: false,
                }, {
                    text: 'TV',
                    url: '#',
                    current: false,
                }, {
                    text: 'GAMES',
                    url: '#',
                    current: false,
                }, {
                    text: 'COLLECTIBLES',
                    url: '#',
                    current: false,
                }, {
                    text: 'VIDEOS',
                    url: '#',
                    current: false,
                }, {
                    text: 'FANS',
                    url: '#',
                    current: false,
                }, {
                    text: 'NEWS',
                    url: '#',
                    current: false,
                }, {
                    text: 'SHOP',
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
            <!-- Logo -->
            <div id="headerLogo">
                <a href="#">
                    <img src="../assets/img/dc-logo.png" alt="">
                </a>
            </div>
            <!-- Nav Menu -->
            <nav>
                <ul>
                    <li v-for="(link, idx) in links" :key="idx" :class="link.current ? 'active' : ''">
                        <a :href="link.url">
                            {{ link.text }}
                        </a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;

.container {
    justify-content: space-between;
}

#headerLogo {
    height: 75px;
    padding: 15px 0;
}

a {
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100%;
}

ul {
    display: flex;
    gap: 10px;
    height: 100%;

    a {
        height: 75px;
    }

    li.active,
    li:hover {
        color: #0678db;
    }

    li.active {
        border-bottom: 4px solid #0678db;
    }

}
</style>
