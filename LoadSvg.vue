<template>
	<div class="rawsvg" v-html="svg"></div>
</template>

<script setup>
import { onMounted, ref } from 'vue';

const props = defineProps({
	name: {
		type: String,
		required: true,
	},
});

let svg = ref('');

onMounted(async () => {
	// Only from puclic directory
	const res = await fetch(`/svg/${props.name}.svg?raw`);
	svg.value = await res.text();	
});
</script>
