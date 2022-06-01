<template>
  <main>
    <div class="container">
        <h2> --> Content goes here </h2>
    </div>
  </main>
</template>

<script>
export default {
    name: 'BaseMain'
}
</script>

<style lang="scss">
    main{

        background-color: var(--main-bg-color);

        & h2{
            color: #fff;
            padding: 3.125rem 0;
        }
    }

</style>