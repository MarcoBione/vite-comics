<template>
    <main>
        <!-- first part -->
        <div class="text-bg-dark p-3">
            <div class="container">
                <!-- rows -->
                <div class="row">
                    <!-- columns -->
                    <div class="col col-12 col-sm-6 col-md-4 col-lg-3" v-for="menu, index in linkMenu" :key="index">
                        <!-- single card -->
                        <div class="card bg-transparent border-light">
                            <!-- image card -->
                            <img :src="menu.thumb" class="card-img-top img-fluid" alt="menu.type">
                            <!-- title of the movie -->
                            <div class="card-body h-25">
                                <h5 class="card-title text-white fw-semibold m-0">{{ menu.series }}</h5>
                            </div>

                        </div>

                    </div>

                </div>

            </div>
        </div>

        <!-- second part -->
        <div class="text-bg-primary">
            <div class="container">
                <ul class="d-flex list-unstyled p-3 justify-content-between m-0">
                    <li v-for="(item, index) in linkBar" @key='index'
                        class="fw-semibold text-uppercase d-flex align-items-center _mypointer">
                        <img :src="item.link" :alt="item.name" class="_myimg">
                        <p class="m-0 px-2 w-100">{{ item.name }}</p>
                    </li>
                </ul>
            </div>

        </div>
    </main>
</template>

<script>
export default {
    data() {
        return {

            linkBar: [
                {
                    name: 'Digital Comics',
                    link: '/buy-comics-digital-comics.png'
                },
                {
                    name: 'DC Merchandise',
                    link: '/buy-comics-merchandise.png'
                },
                {
                    name: 'subscription',
                    link: '/buy-comics-subscriptions.png'
                },
                {
                    name: 'comic shop locator',
                    link: '/buy-comics-shop-locator.png'
                },
                {
                    name: 'Dc power visa',
                    link: '/buy-dc-power-visa.svg'
                }
            ],
            linkMenu: [
                {
                    "thumb": "https://m.media-amazon.com/images/I/51f+H6WXoCL.jpg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://mlpnk72yciwc.i.optimole.com/cqhiHLc.IIZS~2ef73/w:auto/h:auto/q:75/https://bleedingcool.com/wp-content/uploads/2021/05/AQM_80THANN_Cv11_60a2d6ea2f7545.69069474-1.jpg",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://upload.wikimedia.org/wikipedia/it/1/19/Batman_3_variant.jpg",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://m.media-amazon.com/images/M/MV5BZjdjN2VjMDQtZjc2Ni00ZTIxLWIzYjktOTE0MTY3ZTFiNGZiXkEyXkFqcGdeQXVyMjI4OTg3MTc@._V1_FMjpg_UX1000_.jpg",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BTMA017_0.jpg",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://m.media-amazon.com/images/W/IMAGERENDERING_521856-T1/images/I/51adBmhyprL.jpg",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://m.media-amazon.com/images/W/IMAGERENDERING_521856-T1/images/I/41nGyVF7C2L.jpg",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://m.media-amazon.com/images/I/51ZiSKqSRAL.jpg",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://m.media-amazon.com/images/I/51IktbDrQ9L.jpg",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/m/1/m1blin055isbn_0.jpg",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ]

        }
    }
}
</script>

<style lang="scss" scoped></style>