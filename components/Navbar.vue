<template>
  <div class=" bg-white px-4 py-4 flex justify-between w-full">
      <div class=" lg:flex items-center">
          <ul class="flex flex-col lg:flex-row list-none ml-auto">
            <li class="nav-item">
                <nuxt-link to="/" class="mx-3 py-2 flex items-center text-sm uppercase font-bold leading-snug text-gray-900 hover:opacity-75" >
                <span>Home</span>
                </nuxt-link>
            </li>
            <li class="nav-item">
                <nuxt-link to="/about-us" class="mx-3 py-2 flex items-center text-sm uppercase font-bold leading-snug text-gray-900 hover:opacity-75" >
                <span>About Us</span>
                </nuxt-link>
            </li>
            <li class="nav-item">
                <nuxt-link to="/services" class="mx-3 py-2 flex items-center text-sm uppercase font-bold leading-snug text-gray-900 hover:opacity-75" >
                <span>Services</span>
                </nuxt-link>
            </li>
            <li class="nav-item">
                <nuxt-link to="/projects" class="mx-3 py-2 flex items-center text-sm uppercase font-bold leading-snug text-gray-900 hover:opacity-75" >
                <span>Projects</span>
                </nuxt-link>
            </li>
            <li class="nav-item">
                <nuxt-link to="/contact-us" class="mx-3 py-2 flex items-center text-sm uppercase font-bold leading-snug text-gray-900 hover:opacity-75" >
                <span>Contact Us</span>
                </nuxt-link>
            </li>
          </ul>
      </div>

      <div class=" flex">
         <div class=" w-14 border-l border-black flex justify-center items-center">
             <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-black" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 8h10M7 12h4m1 8l-4-4H5a2 2 0 01-2-2V6a2 2 0 012-2h14a2 2 0 012 2v8a2 2 0 01-2 2h-3l-4 4z" />
            </svg>
         </div>
         <div class=" w-14 border-l border-black flex justify-center items-center">
             <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-black" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 8h10M7 12h4m1 8l-4-4H5a2 2 0 01-2-2V6a2 2 0 012-2h14a2 2 0 012 2v8a2 2 0 01-2 2h-3l-4 4z" />
            </svg>
         </div>
         <div class=" w-14 border-l border-black flex justify-center items-center">
             <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-black" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 8h10M7 12h4m1 8l-4-4H5a2 2 0 01-2-2V6a2 2 0 012-2h14a2 2 0 012 2v8a2 2 0 01-2 2h-3l-4 4z" />
            </svg>
         </div>
         <div class=" w-14 border-l border-black flex justify-center items-center">
             <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-black" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 8h10M7 12h4m1 8l-4-4H5a2 2 0 01-2-2V6a2 2 0 012-2h14a2 2 0 012 2v8a2 2 0 01-2 2h-3l-4 4z" />
            </svg>
         </div>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
.nuxt-link-exact-active {
  @apply text-yellow-500;
}

</style>