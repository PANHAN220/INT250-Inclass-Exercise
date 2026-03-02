<script setup>
 defineProps({
    title: String,
    storage: String,
    price: Number,
    features: Array
 })

</script>

<template>
    <!-- Card -->
    <div class="group bg-[#1E293B] w-64 rounded-lg p-6 text-white shadow-lg border-8 border-gray-500 hover:border-violet-500 transition">
        
        <!-- Title -->
        <div class="text-center text-sm mb-4">
            <h3>{{title}}</h3>
        </div>


        <!-- Storage -->
        <div class="text-center text-4xl mb-4 font-serif">
            <h1>{{storage}}</h1>
        </div>

        <!-- Prize -->
        <div class="text-center text-sm mb-6">
            <h3>${{ price }}/month</h3>
        </div>

        <!-- Purchase -->
        <div class="mb-10 ">
            <button class="block mx-auto w-40 border-2 border-violet-500 py-1.5 rounded-lg group-hover:bg-violet-500 transition ">Purchase</button>
        </div>

        <hr class="my-6 border-gray-600 -mx-6">

        <!-- Feature -->
        <ul class="text-center space-y-1">
            <li v-for="item in features" >
                ✓ {{ item }}
            </li>
            

            <!-- <li v-for="item in features":key="item.title" v-bind="item">
                ✓ {{ item }}
            </li> -->

            <!-- <li v-for="(item, index) in features" :key="index">
                ✓ {{ item }}
            </li> -->
        </ul>

    </div>

</template>

<style scoped></style>
