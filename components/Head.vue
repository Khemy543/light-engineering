<template>
  <div class=" w-full relative shadow-md h-screen bg-black">
        <img src="~/static/images/umit-yildirim-9OB46apMbC4-unsplash.jpg" alt="" class=" carousel-image object-cover w-full h-full">
        <div class="content w-full max-w-6xl mx-auto overflow-hidden">
            <Navbar />
        </div>
        <div class=" text-content">  
            <div class=" text-4xl uppercase font-extrabold text-white text-center">{{head}}</div>
            <div class=" text-base font-normal uppercase text-white text-center mt-10">{{text}}</div>
        </div>
  </div>
</template>

<script>
export default {
    props : ["image", "text", "head"]
}
</script>

<style>
</style>