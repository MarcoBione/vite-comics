<template>
    <main>
        <!-- first part -->
        <div class="text-bg-dark">
            <div class="container">
                <h2 class="m-0">---Content Goes Here---</h2>
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

        }
    }
}
</script>

<style lang="scss" scoped></style>