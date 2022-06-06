<template>
  <section class="main-hero"></section>
</template>

<script>
export default {
    name: "MainHero"
}
</script>

<style lang="scss">
    .main-hero{
        min-height: 20vw;
        background-position: top;
        background-size: cover;
        background-image: var(--main-hero-img);
    }
</style>