<template>
    <footer>

        <!-- footer top -->
        <div class="bg-dark _myfooter p-3">
            <div class="container d-flex justify-content-between">

                <!-- links -->
                <div class="links">

                    <!-- title of the link list -->
                    <ul class="fs-semibold text-white list-unstyled d-flex">

                        <!-- cycle for title list rendering -->
                        <li v-for="item, index in linksData" :key="index" class="px-3">

                            <h4 class="fw-semibold">{{ item.category }}</h4> <!-- title rendering -->

                            <!-- rendering for all links inside obj -->
                            <ul v-for="link, index in item.links" :key="index" class="p-0">
                                <li class="list-unstyled">
                                    <p class=" _mypointer _mylinks m-0">{{ link.name }}</p>
                                    <!-- rendering of all links inside 'categories' -->
                                </li>
                            </ul>
                            <!-- end rendering for all links inside obj -->

                        </li>
                        <!-- end cycle for title list rendering -->

                    </ul>
                    <!-- end title of the link list -->

                </div>
                <!-- end links -->

                <!-- logo -->
                <div class="logo">
                    <img class="_mybglogo" src="/dc-logo-bg.png" alt="dc-logo">
                </div>

            </div>
        </div>

        <!-- footer bottom -->
        <div class="bg-dark">
            <div class="container p-2 d-flex justify-content-between">
                <!-- button -->
                <div class="d-flex align-items-center">
                    <button class="_mybtn">Sign Up now</button>
                </div>

                <!-- socials -->
                <div class="p-2">
                    <ul class="d-flex list-unstyled m-0 align-items-center">
                        <li class="px-1 text-uppercase text-primary fw-semibold">Follow us</li>
                        <li class="px-1"><img src="/footer-facebook.png" alt="facebook-logo"></li>
                        <li class="px-1"><img src="/footer-twitter.png" alt="twitter-logo"></li>
                        <li class="px-1"><img src="/footer-youtube.png" alt="youtube-logo"></li>
                        <li class="px-1"><img src="/footer-pinterest.png" alt="pinterest-logo"></li>
                        <li class="px-1"><img src="/footer-periscope.png" alt="periscope-logo"></li>
                    </ul>
                </div>
            </div>
        </div>

    </footer>
</template>

<script>
export default {
    data() {
        return {
            linksData: [
                {
                    category: 'Dc comics',
                    links: [
                        {
                            name: 'Characters',
                            link: '#',
                        },
                        {
                            name: 'Comics',
                            link: '#',
                        },
                        {
                            name: 'Movies',
                            link: '#',
                        },
                        {
                            name: 'TV',
                            link: '#',
                        },
                        {
                            name: 'Games',
                            link: '#',
                        },
                        {
                            name: 'Videos',
                            link: '#',
                        },
                        {
                            name: 'News',
                            link: '#',
                        },
                    ]
                },
                {
                    category: 'Shop',
                    links: [
                        {
                            name: 'Shop DC',
                            link: '#',
                        },
                        {
                            name: 'Shop DC Collectibles',
                            link: '#',
                        }
                    ]
                },
                {
                    category: 'DC',
                    links: [
                        {
                            name: 'Therms Of Use',
                            link: '#',
                        },
                        {
                            name: 'Privacy policy (New)',
                            link: '#',
                        },
                        {
                            name: 'Ad Choises',
                            link: '#',
                        },
                        {
                            name: 'Advertising',
                            link: '#',
                        },
                        {
                            name: 'Jobs',
                            link: '#',
                        },
                        {
                            name: 'Subscriptions',
                            link: '#',
                        },
                        {
                            name: 'Talent Workshops',
                            link: '#',
                        },
                        {
                            name: 'CPSC Certificates',
                            link: '#',
                        },
                        {
                            name: 'Ratings',
                            link: '#',
                        },
                        {
                            name: 'Shop Help',
                            link: '#',
                        },
                        {
                            name: 'Contact US',
                            link: '#',
                        },
                    ]
                },
                {
                    category: 'Sites',
                    links: [
                        {
                            name: 'DC',
                            link: '#',
                        },
                        {
                            name: 'MAD Magazines',
                            link: '#',
                        },
                        {
                            name: 'DC Kids',
                            link: '#',
                        },
                        {
                            name: 'DC universe',
                            link: '#',
                        },
                        {
                            name: 'DC Power Visa',
                            link: '#',
                        },
                        {
                            name: 'Subscriptions',
                            link: '#',
                        }
                    ]
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped></style>