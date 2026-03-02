<script setup>
import Cards from './components/Cards.vue';

const plans = [
    {
        title: "Basic",
        storage: "100GB",
        price: "1.99",
        features: [
            "100GB storage",
            "Option to add members",
            "Extra memeber benefits"
        ]
    },
    {
        title: "Standard",
        storage: "200GB",
        price: "3.99",
        features: [
            "200GB storage",
            "Option to add members",
            "Extra memeber benefits"
        ]
    },
    {
        title: "Premium",
        storage: "2TB",
        price: "8.99",
        features: [
            "2TB storage",
            "Option to add members",
            "Extra memeber benefits"
        ]
    }
]
</script>

<template>
    <div class="bg-[#1E293B] min-h-screen flex items-center justify-center gap-8">
        <Cards 
            v-for="plan in plans"
            :key="plan.title"
            v-bind="plan"    
        />
        
    </div>
</template>

<style scoped></style>
