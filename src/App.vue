<template>
    <div class="main-container">
        <NavbarComponent/>
        <HomeView/>
    </div>
</template>

<script>


import HomeView from "@/views/HomeView.vue";
import NavbarComponent from "@/components/NavbarComponent.vue";

export default {
  name: 'App',
  components: {
    NavbarComponent,
    HomeView
  }
}
</script>

<style>
.main-container {
  width: 100%;
  height: 120vh;
}
</style>
