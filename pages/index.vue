<template>
  <div>
    <div class=" py-24  w-full max-w-6xl mx-auto px-4">
    <div class=" text-center">
      <div class=" uppercase text-lg font-semibold">Our Services</div>
      <div class=" mt-2 text-base font-normal uppercase text-gray-700">Years of Experience</div>

      <div class=" flex space-x-10 mt-10">
        <div class=" w-1/3">
          <div class=" h-40 w-40 rounded-full flex justify-center items-center bg-yellow-500 mx-auto">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 8h14M5 8a2 2 0 110-4h14a2 2 0 110 4M5 8v10a2 2 0 002 2h10a2 2 0 002-2V8m-9 4h4" />
          </svg>
          </div>

          <div class=" mt-4 text-base font-semibold text-center">
            3D MODELLING AND AERIAL PHOTOGRAPHY
          </div>

          <p class=" mt-2 text-sm font-normal text-gray-800">We provide Aerial Photography and videography services for real estate marketing, project marketing, events, also generates photo-realistic 3D models (Digital Twin) for engineers,..</p>
        </div>
        <div class=" w-1/3">
          <div class=" h-40 w-40 rounded-full flex justify-center items-center bg-yellow-500 mx-auto">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 8h14M5 8a2 2 0 110-4h14a2 2 0 110 4M5 8v10a2 2 0 002 2h10a2 2 0 002-2V8m-9 4h4" />
          </svg>
          </div>

          <div class=" mt-4 text-base font-semibold text-center">
            AERIAL SURVEYING AND MAPPING
          </div>

          <p class=" mt-2 text-sm font-normal text-gray-800">We provide professional Survey solutions such as Aerial mapping, Stockpile surveys, Topographic Surveys, Production of High resolution Orthophotos,...</p>
        </div>
        <div class=" w-1/3">
          <div class=" h-40 w-40 rounded-full flex justify-center items-center bg-yellow-500 mx-auto">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 8h14M5 8a2 2 0 110-4h14a2 2 0 110 4M5 8v10a2 2 0 002 2h10a2 2 0 002-2V8m-9 4h4" />
            </svg>
          </div>

          <div class=" mt-4 text-base font-semibold text-center">
            DRONE RENTAL SERVICE
          </div>

          <p class=" mt-2 text-sm font-normal text-gray-800">We provide drone rental at affordable rates and we complement our rental service with trained UAV pilots.</p>
        </div>
      </div>
    </div>
  </div>

  <div class="py-24 bg-black">
    <div class=" w-full max-w-6xl mx-auto px-4 text-center">
      <div class=" uppercase text-lg font-semibold text-white">Featured Products</div>
      <div class=" mt-2 text-base font-normal uppercase text-gray-500">WE TAKE PRIDE IN OUR WORK</div>
    
      <div class="grid grid-cols-3 gap-10 mt-10">
        <img src="~/static/images/umit-yildirim-9OB46apMbC4-unsplash.jpg" class=" h-72 w-full object-cover" alt="" v-for="n in 6" :key="n">
      </div>
    </div>
  </div>

  <div class="py-24 max-w-6xl mx-auto px-4 text-center">
      <div class=" uppercase text-lg font-semibold text-black">EXPERT TEAM</div>
      <div class=" mt-2 text-base font-normal uppercase text-gray-700">Lorem ipsum dolor sit amet, consectetur adipiscing elit</div>
  
      <div class=" flex mt-10 space-x-20 w-full">
        <div>
          <img src="~/static/images/umit-yildirim-9OB46apMbC4-unsplash.jpg" alt="" class=" h-52 w-full">
          <div class=" py-5">
              <div class=" text-base font-semibold">Lorains Methw</div>
              <p class="text-sm font-normal">Architecture Designer</p>
          </div>
        </div>
        <div>
          <img src="~/static/images/umit-yildirim-9OB46apMbC4-unsplash.jpg" alt="" class=" h-52 w-full">
          <div class=" py-5">
              <div class=" text-base font-semibold">Lorains Methw</div>
              <p class="text-sm font-normal">Architecture Designer</p>
          </div>
        </div>
        <div>
          <img src="~/static/images/umit-yildirim-9OB46apMbC4-unsplash.jpg" alt="" class=" h-52 w-full object-cover">
          <div class=" py-5">
              <div class=" text-base font-semibold">Lorains Methw</div>
              <p class="text-sm font-normal">Architecture Designer</p>
          </div>
        </div>
      </div>
  </div>

  <div class=" bg-gray-200 ">
    <div class=" max-w-6xl mx-auto px-4 text-center py-24">
      <div class=" uppercase text-lg font-semibold text-black">CLIENT'S TESTIMONIAL</div>
      <div class=" mt-28 border border-gray-700 rounded px-28 py-28 relative">
        <img src="~/static/images/umit-yildirim-9OB46apMbC4-unsplash.jpg" alt="" 
          class=" absolute h-24 w-24 rounded-full object-cover -top-12" style="right:46%" />

          <p class=" font-normal text-sm ">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus rutrum scelerisque porta. Nam quis . Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus rutrum scelerisque porta. Nam quis . Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus rutrum scelerisque porta. Nam quis . Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus rutrum scelerisque porta. Nam quis
          </p>
      </div>
    </div>
  </div>
  </div>
</template>

<script>
export default {
}
</script>
