<script setup>
    import { ref } from 'vue'

    import image1 from '../assets/image1.jpg'
    import image2 from '../assets/image2.jpg'
    import image3 from '../assets/image3.jpg'
    import image4 from '../assets/image4.jpg'
    import image5 from '../assets/image5.jpg'
    import image6 from '../assets/image6.jpg'

    const images = ref([
    { id: 1, url: image1 },
    { id: 2, url: image2 },
    { id: 3, url: image3 },
    { id: 4, url: image4 },
    { id: 5, url: image5 },
    { id: 6, url: image6 }
    ])
</script>

<template>
    <div class="max-w-6xl mx-auto">
        <!-- Navbar -->
    
         <div class="flex justify-end space-x-8 py-6 text-xl">
            <button class="hover:font-medium transition duration-300">Vector</button>
            
            <button class="hover:font-medium transition duration-300">Illustrations</button>
    
            <button class="hover:font-medium transition duration-300">Images</button>
    
            <button class="hover:font-medium transition duration-300">Icons</button>
         </div>
    

         <div class="flex items-end justify-between gap-6">    
             <!-- Search -->
              <div class="relative flex-1 max-w-md">
                <input type="text" placeholder="Search" class="w-full border-b border-gray-300 py-4 pl-2 text-xl my-4 ">
                <i class="fa-solid fa-magnifying-glass absolute right-4 top-1/2 -translate-y-1/2 text-gray-400"></i>
              </div>
                
             <button class="bg-black  text-white text-xl py-4 px-16 my-4 rounded-2xl">Upload</button>
         </div>

         <!-- image zone-->

           <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6 mt-10">
                <div v-for="img in images" :key="img.id" class="overflow-hidden hover:transition duration-300">
                    <img :src="img.url" class="w-full h-60 object-cover hover:scale-110 transition duration-300"/>
                </div>
         </div>
    </div>
</template>