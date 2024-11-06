<script setup>
import teaching from '@/assets/teaching.jpg'
import nonteaching from '@/assets/non-teaching.jpg'
import principal from '@/assets/principal.jpeg'
</script>
<template>
    <AppHeader />
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 mb-12">
        <h2 class="text-2xl p-2 px-8">Principal</h2>
		<p class="text-xl p-2 px-8 border-b-2">Dr. Kailash yadav<br /><span class="text-sm"><a :href="principal" target="_blank">Click to see univeristy Approval</a></span></p>
		<h2 class="text-2xl p-2 px-8 border-b-2">Teaching Staff</h2>
		<img :src="teaching" />

        <h2 class="text-2xl p-2 px-8 border-b-2">Non-Teaching Staff</h2>
		<img :src="nonteaching" />

    </div>
    <Footer />
</template>
