<template>
    <header>

        <!-- logo DC -->
        <div class="logo">
            <img src="../assets/vue-dc-comics-1/img/favicon.ico" alt="dc_logo">
        </div>
        <!-- nav bar commands -->
        <nav>
            <ul class="d-flex list-unstyled">
                <li v-for="(item, index) in navBar" @key='index' class="_myitem">
                    {{ item.name }}
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