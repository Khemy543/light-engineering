<template>
  <div>
      <Header />
      <Carousel />
      <div>
          <Nuxt />
      </div>
      <Footer />
  </div>
</template>

<script>
export default {
    components:{
        Header : () => import('~/components/Header.vue'),
        Carousel : () => import('~/components/Carousel.vue'),
        Footer : () => import('~/components/Footer.vue')
    }
}
</script>

<style>

</style>