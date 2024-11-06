<script setup>
import { GoogleMap, Marker } from 'vue3-google-map'
const mapApi = ref(import.meta.env.VITE_MAPKEY)
const center = { lat: 28.377285, lng: 75.411813 }
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
        <Marker :options="{ position: center, title: 'Malaram Kothari Teachers Training College' }" />
    </GoogleMap>
    <h2 class="text-2xl p-2 px-8 border-b-2">Contact Info:</h2>
    <p class="text-lg font-bold px-8">Malaram Kothari Teachers Training College</p>
    <p class="text-lg px-8">Rajgarh Road, Sankhantal</p>
	<p class="text-lg px-8">Teh. Rajgarh, Dist. Churu, Rajasthan</p>
	<p class="text-lg px-8">Phone: +91-9414540356</p>
    </div>
    <Footer />
</template>
