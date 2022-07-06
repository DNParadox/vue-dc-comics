<template>
    <footer>
        <div class="container">

            <div class="container-ul">
                <div v-for="(element, index) in liContent" :key="index" class="column">
                    <div class="column-title"> {{ element.title }} </div>
                    <ul v-for="(message, index) in liContent[index].allText" :key="index" class="footerul">
                        <li><a :href="element.url"> {{ message.text }} </a></li>

                    </ul>
                </div>

         
            
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'dcFooter',
    data() {
        return {
            liContent: [
                {
                    title: 'DC COMICS',
                    url: '#',
                    allText: [
                        {
                            text: 'Characters',
                        },
                        {
                            text: 'Comics',
                        },
                        {
                            text: 'Movies',
                        },
                        {
                            text: 'TV',
                        },
                        {
                            text: 'Games',
                        },
                        {
                            text: 'Videos',
                        },
                        {
                            text: 'News',
                        },
                    ],
                },
                {
                    title: 'DC',
                    url: '#',
                    allText: [
                                       {
                            text: 'Terms of Use',
                        },
                        {
                            text: 'Privacy Policy(New)',
                        },
                        {
                            text: 'Ad Choices',
                        },
                        {
                            text: 'Advertising',
                        },
                        {
                            text: 'Jobs',
                        },
                        {
                            text: 'Subscriptions',
                        },
                        {
                            text: 'Talent Workshops',
                        },
                        {
                            text: 'CPCS Certificates',
                        },
                        {
                            text: 'Ratings',
                        },
                        {
                            text: 'Shop Help',
                        },
                        {
                            text: 'Contact Us',
                        },
                    ],
                },
                {
                    title: 'SITES',
                    url: '#',
                    allText: [
                        {
                            text: 'DC',
                        },
                        {
                            text: 'MAD Magazine',
                        },
                        {
                            text: 'DC Kids',
                        },
                        {
                            text: 'DC Universe',
                        },
                        {
                            text: 'DC Power Visa',
                        },
                       
                    ],
                },
                {
                    title: 'SHOP',
                    url: '#',
                    allText: [
                        {
                            text: 'test',
                        },
                        {
                            text: 'prova',
                        }
                    ],
                },

            ]
        }

    }
}


</script>

<style scoped lang="scss">
@import '../style/variables.scss';

footer {
    background-image: url(../assets/img/footer-bg.jpg);
    height: 300px;
    color: $brand_secondary_color;

    .container-ul {
        padding-top: 40px;
        display: flex;
        justify-content: space-around;
        width: 400px;

        .footerul {
            padding-top: 10px;
        }
        a {
            color: white
        }
    }
}
</style>