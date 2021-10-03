<template>
  <div class=" w-full">
      <Header />
      <Head
        :head="routeName"
        :text="text"
      />
      <div class=" py-20 w-full">
          <Nuxt />
      </div>
      <Footer />
  </div>
</template>

<script>
export default {
    components : {
        Header : () => import('~/components/Header.vue'),
        Head : () => import('~/components/Head.vue'),
        Footer : () => import('~/components/Footer.vue')
    },
    computed : {
        routeName(){
            return this.$route.name.replace(/-/g, ' ')
        },
        text(){
            return this.routeName === 'about us' ? 'who are we' 
            :this.routeName === 'services' ? 'years of experience'
            :this.routeName === 'projects' ? 'we take pride in our work'
            :this.routeName === 'contact us' ? "got a question or concern? let's get in touch" : null 
        }
    }
}
</script>

<style>

</style>