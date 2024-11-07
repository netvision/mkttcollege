<script setup>
import PDF from "pdf-vue3";
</script>

<template>
	<AppHeader />
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 mb-12">
		<ul class="text-xl p-2 px-8">
			<PDF src="./students-22-23.pdf" />
		</ul>
    </div>
    <Footer />
</template>
