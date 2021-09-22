<template>
  <div class=" w-full h-screen carousel relative shadow-2xl bg-white">
    <div class=" carousel-inner relative overflow-hidden w-full h-full">

      <div class=" w-full h-full">
        <input class="carousel-open" type="radio" id="carousel-1" name="carousel" aria-hidden="true" hidden="" checked>
        <div class=" carousel-item absolute opacity-0 w-full h-full">
          <div class=" block w-full h-full bg-black text-white text-center">
            <img src="~/static/images/umit-yildirim-9OB46apMbC4-unsplash.jpg" alt="" class=" object-cover w-full h-full carousel-image">
            <div class="content w-full max-w-6xl mx-auto overflow-hidden">
              <Navbar />
            </div>
              <div class=" text-content">  
                <div class=" text-sm font-normal uppercase text-white">Build with Osono</div>
                <div class=" text-4xl uppercase font-extrabold text-white mt-10">We Build Great Projects</div>
              </div>

              <button class=" bottom bg-yellow-500  text-black rounded px-5 py-4 uppercase text-sm font-semibold">
                Who are we
              </button>
          </div>
        </div>
      </div>

      <ol class="carousel-indicators">
			<li class="inline-block mr-3">
				<label for="carousel-1" class="carousel-bullet cursor-pointer block text-4xl text-white hover:text-blue-700">•</label>
			</li>
			<li class="inline-block mr-3">
				<label for="carousel-2" class="carousel-bullet cursor-pointer block text-4xl text-white hover:text-blue-700">•</label>
			</li>
      <li class="inline-block mr-3">
				<label for="carousel-3" class="carousel-bullet cursor-pointer block text-4xl text-white hover:text-blue-700">•</label>
			</li>
		</ol>

    </div>
  </div>
</template>

<script>
export default {
  components:{
        Navbar : () => import('~/components/Navbar.vue')
  }
}
</script>

<style>
.carousel-open:checked + .carousel-item {
  position: static;
  opacity: 100;
}
.carousel-item {
  -webkit-transition: opacity 0.6s ease-out;
  transition: opacity 0.6s ease-out;
}
#carousel-1:checked ~ .control-1,
#carousel-2:checked ~ .control-2,
#carousel-3:checked ~ .control-3 {
  display: block;
}
.carousel-indicators {
  list-style: none;
  margin: 0;
  padding: 0;
  position: absolute;
  bottom: 2%;
  left: 0;
  right: 0;
  text-align: center;
  z-index: 10;
}
#carousel-1:checked ~ .control-1 ~ .carousel-indicators li:nth-child(1) .carousel-bullet,
#carousel-2:checked ~ .control-2 ~ .carousel-indicators li:nth-child(2) .carousel-bullet,
#carousel-3:checked ~ .control-3 ~ .carousel-indicators li:nth-child(3) .carousel-bullet {
  color: #2b6cb0;  /*Set to match the Tailwind colour you want the active one to be */
}
.carousel-image {
		opacity : 0.3;
}

.content{
  position: absolute;
  top: 28%;
  left: 50%;
  transform: translate(-50%, -50%);
  color: white;
}

.text-content{
  position: absolute;
  top:50%;
  left:50%;
  transform: translate(-50%, -50%);
}

.bottom { 
  position: absolute;
  top:75%;
  left:50%;
  transform: translate(-50%, -50%);

}

.inner-height{
  height: 75vh;
}
</style>