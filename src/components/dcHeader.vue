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
                    <li v-for="link, index in menuLinks" :key="index" :class="{ 'current': link.current }">
                        <a :href="link.url">{{ link.text }}</a>
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

<style lang="scss">

header {
    height: 100px;
    // Container modificato
    .container {
    margin: 30px auto;
}
   
    // Logo
    .logo {
        text-align: center;
        img {
            width: 80px;
            height: 80px;
            display: block;
        }
    }

 .menu {
        margin: 30px 0;
        display: flex;
        justify-content: center;
        li {
            padding: 10px;
            a {
                color: black;
                text-decoration: none;
                font-size: 1.2rem;
            }
            &.current {
                background-color: red;
            }
        }
    }
}


</style>