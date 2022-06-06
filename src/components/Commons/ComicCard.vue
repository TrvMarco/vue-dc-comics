<template>
  <div class="comic-card">
      <img :src="image" :alt="title">
      <h4>{{title}}</h4>
  </div>
</template>

<script>
export default {
    name: 'ComicCard',
    props: {
        image: String,
        title: String
    }
}
</script>

<style lang="scss">
    .comic-card{
        & img{
            width: 100%;
            height: 200px;
            object-fit: cover;
            object-position: top;
        }

        & h4{
            color: #fff;
            text-transform: uppercase;
            font-weight: 500;
            font-size: .9375rem;
        }
    }
</style>