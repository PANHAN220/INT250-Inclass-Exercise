<script setup></script>

<template>
    <!-- Background Container -->
    <div class="flex items-center justify-center bg-zinc-700 min-h-screen">
        <!-- Card -->
         <div class="bg-zinc-800 p-2 mx-1 rounded-2xl">
            <!-- Flex Container -->
             <div class="flex flex-col md:flex-row rounded-l-xl">
                <!-- image -->
                <img src="../assets/dietfood.jpg" alt="" class="object-fit rounded-xl h-80 
                md:h-64 rounded-l-xl md:rounded-r-none transform hover:scale-105 hover:rounded-xl duration-200">

                <!-- Content -->
                 <div class="text-white flex flex-col justify-center p-6 space-y-2">
                    <h2 class="font-serif text-xl font-medium text-center md:text-left">Get diet and fitness tips in your inbox</h2>

                    <p class="max-w-xs text-xs text-center leading-5 tracking-wide md:text-left">Eat better and exercise better Sign up for the Diet&fitness newsletter</p>

                    <div class="flex flex-col mt-5 space-y-4 md:space-x-3 md:flex-row md:space-y-0">
                        <input type="text" placeholder="Enter your email Address" class="p-2 px-6 text-center
                        text-white bg-zinc-800 border border-zinc-600 placeholder:text-xs placeholder:text-center
                        md:text-left placeholder:md:text-left focus:outline-none"/>
                        <button class="text-zinc-700 bg-lime-500 hover:bg-lime-700 rounded-md hover:text-white  duration-500 ">
                            <p class="text-xs m-2">Subscribe</p>
                        </button>
                    </div>
                 </div>
                    
             </div>
         </div>

    </div>
</template>

<style scoped>


</style>
