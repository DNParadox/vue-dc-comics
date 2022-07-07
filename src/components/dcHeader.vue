<template>
    <!-- header -->
    <header>
        <div class="container">
                    <!-- logo -->
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="logo DC">
            </div>

            <nav>
                <ul class="menu">
                    <li v-for="link, index in menuLinks" :key="index" :class="{'current': link.current}" >
                        <a :class="{'current': link.current}" :href="link.url">{{ link.text }}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>


<script>
export default {
  name: 'dcHeader',
    data() {
        return {
            menuLinks: [
                {
                    text: 'Characters',
                    url: '#',
                    current: false
                },
                {
                    text: 'Comics',
                    url: '#',
                    current: true
                },
                {
                    text: 'Movies',
                    url: '#',
                    current: false
                },
                {
                    text: 'Collectibles',
                    url: '#',
                    current: false
                },
                  {
                    text: 'Collectibles',
                    url: '#',
                    current: false
                },
                {
                    text: 'Videos',
                    url: '#',
                    current: false
                },
                {
                    text: 'Fans',
                    url: '#',
                    current: false
                },
                {
                    text: 'News',
                    url: '#',
                    current: false
                },
                {
                    text: 'Shop',
                    url: '#',
                    current: false
                },
            ],
        };
    }
}
  
</script>

<style  scoped lang="scss">
@import '../style/variables.scss';
header {
    background-color: $brand_secondary_color;
    height: 100px;
    // Container modificato
    .container {
        height: 100%;
}
    .logo {
        height: 100%;
        display: flex;
        align-items: center;
        img {
            width: 80px;
            height: auto;
            display: block;
        }
    }
 .menu {
    display: flex;
    justify-content: center;
    height: 100%;
    align-items: center;
        li {
            padding-left: 10px;
            a {
                color: black;
                text-decoration: none;
                font-size: 1.2rem;
                &.current {
                    color: $brand_main_color;       
                }
             }
        }
    }
}
</style>