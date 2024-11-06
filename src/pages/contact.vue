<script setup>
import { GoogleMap, Marker } from 'vue3-google-map'
const mapApi = ref(import.meta.env.VITE_MAPKEY)
const center = { lat: 28.314596, lng: 75.4322150 }
</script>
<template>
    <AppHeader />
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 mb-12">
    <GoogleMap
    :api-key="mapApi"
    style="width: 100%; height: 500px"
    :center="center"
    :zoom="16"
    >
        <Marker :options="{ position: center, title: 'Kothari Mahila Mahavidyalay' }" />
    </GoogleMap>
    <h2 class="text-2xl p-2 px-8 border-b-2">Contact Info:</h2>
    <p class="text-lg font-bold px-8">Kothari Mahila mahavidyalaya</p>
    <p class="text-lg px-8">Ward No. 15, Mandrella-333025,</p>
	<p class="text-lg px-8">Teh. Chirawa, Dist. Jhunjhunu, Rajasthan</p>
	<p class="text-lg px-8">Phone: +91-9929247066</p>
    </div>
    <Footer />
</template>
