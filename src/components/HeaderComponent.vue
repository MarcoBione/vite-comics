<template>
    <header>
        <!-- nav bar commands -->
        <nav class="d-flex container justify-content-between align-items-center py-4">
            <!-- logo DC -->
            <div>
                <img class="_mylogo" src="/dc-logo.png" alt="dc_logo">
            </div>

            <ul class="d-flex list-unstyled">
                <li v-for="(item, index) in navBar" @key='index' class="px-3 fw-semibold text-uppercase">
                    <p class="_mynavlink">{{ item.name }}</p>
                </li>
            </ul>

        </nav>

    </header>
</template>

<script>

export default {
    name: 'HeaderComponent',
    data() {
        return {
            navBar: [
                {
                    name: 'Characters',
                    link: '#'
                },
                {
                    name: 'Comics',
                    link: '#'
                },
                {
                    name: 'Movies',
                    link: '#'
                },
                {
                    name: 'TV',
                    link: '#'
                },
                {
                    name: 'Games',
                    link: '#'
                },
                {
                    name: 'Collectibles',
                    link: '#'
                },
                {
                    name: 'Videos',
                    link: '#'
                },
                {
                    name: 'Fans',
                    link: '#'
                },
                {
                    name: 'News',
                    link: '#'
                },
                {
                    name: 'Shop',
                    link: '#'
                },
            ],

        }
    }
}
</script>

<style lang="scss" scoped></style>