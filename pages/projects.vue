<template>
  <div class=" max-w-6xl mx-auto px-4">
      <Tab 
        :tabs="tabs"
        :activeTab="activeTab"
        :changeTab="changeTab"
      />

      <div class=" mt-20 grid grid-cols-3 gap-10">
          <div v-for="n in 9" :key="n">
              <img src="~/static/images/drone.jpeg" alt="drone">
          </div>
      </div>
  </div>
</template>

<script>
export default {
    layout:"others",
    components : {
        Tab : () => import('~/components/Tab.vue')
    },
    data(){
        return{
            tabs : [
                {
                    id:1,
                    name :"All Groups"
                },
                {
                    id:2,
                    name :"Education"
                },
                {
                    id:3,
                    name:"Hospital"
                },
                {
                    id:4,
                    name :"Office"
                },
                {
                    id:5,
                    name :"Residential"
                }
            ],
            activeTab : 1
        }
    },
    methods : {
        changeTab(id){
            this.activeTab = id;
        }
    }
}
</script>

<style>

</style>