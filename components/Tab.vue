<template>
  <div class=" w-full flex justify-center">
    <div class="">
      <ul class="list-reset flex p-1">
        <li class="p-0 mb-0" v-for="tab in tabs" :key="tab.id"
            @click="changeTab(tab.id)">
          <h1
            class="text-sm inline-block px-14 cursor-pointer font-bold py-4"
            :class="activeTab == tab.id ? ' border-b-4 border-yellow-500':null"
            id="1"
          >
            {{tab.name}}
          </h1>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
    props:['activeTab', 'tabs', 'changeTab']
};
</script>

<style></style>
