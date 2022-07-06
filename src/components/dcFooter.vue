<template>
    <footer>
     <div class="footerTop">
           <div class="container">
            <div class="container-ul">
                <div v-for="(element, index) in liContent" :key="index" class="column">
                    <div class="column-title"> {{ element.title }} </div>
                    <ul class="footerul">
                        <li  v-for="(message, index) in liContent[index].allText" :key="index">
                            <a :href="element.url"> {{ message.text }} </a>
                        </li>

                    </ul>
                </div>
            </div>

           <div class="container-logo">
                <img src="../assets/img/dc-logo-bg.png" alt="">
           </div>
        </div>
     </div>

     <div class="footerBottom">
        <div class="container">

            <div class="button">
                  <a href="#">SIGN UP NOW </a>
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
                            text: 'Shop DC',
                        },
                        {
                            text: 'Shop DC Collectible',
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
    height: 380px;
    color: $brand_secondary_color;
    .container-ul {
        padding-top: 40px;
        display: flex;
        justify-content: space-between;
        width: calc(100% / 3);
        flex-wrap: wrap;
        .footerul {
            padding-top: 10px;
        }
            a {
                color: #7d8688;
                font-size: 0.7rem;
            }
    }
}

.column-title{
    color: $brand_secondary_color;
}
img {
    width: 400px;
}

.footerTop {
    height:100%;
}
.footerBottom {
    background-color: #303030;
    height: 100px;
    .container {
        height: 100%;
    }
    .button {
        display: flex;
        align-items: center;
        height: 100%;
        a {
            padding: 10px;
            border: 1px solid #0282f9;
        }
    }
}
</style>