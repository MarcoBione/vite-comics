<template>
  <div>
    <!-- header -->
    <HeaderComponent />
    <!-- main -->
    <MainComponent />
    <!-- Footer -->
    <FooterComponent />
  </div>
</template>

<script>
//components import
import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
import FooterComponent from './components/FooterComponent.vue';

export default {
  components: {
    HeaderComponent,
    MainComponent,
    FooterComponent,
  }
}
</script>

<style lang="scss" scoped></style>
