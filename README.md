# Css
Css styles.

## Glue

```css
:root {
	--glue-grey-0: #fff;
	--glue-grey-25: #f1f1f1;
	--glue-grey-50: #f8f9fa;
	--glue-grey-100: #f1f3f4;
	--glue-grey-200: #e8eaed;
	--glue-grey-300: #dadce0;
	--glue-grey-400: #bdc1c6;
	--glue-grey-500: #9aa0a6;
	--glue-grey-600: #80868b;
	--glue-grey-700: #5f6368;
	--glue-grey-800: #3c4043;
	--glue-grey-900: #202124;
	--glue-blue-50: #e8f0fe;
	--glue-blue-100: #d2e3fc;
	--glue-blue-200: #aecbfa;
	--glue-blue-300: #8ab4f8;
	--glue-blue-400: #669df6;
	--glue-blue-500: #4285f4;
	--glue-blue-600: #1a73e8;
	--glue-blue-700: #1967d2;
	--glue-blue-800: #185abc;
	--glue-blue-900: #174ea6;
	--glue-green-50: #e6f4ea;
	--glue-green-100: #ceead6;
	--glue-green-200: #a8dab5;
	--glue-green-300: #81c995;
	--glue-green-400: #5bb974;
	--glue-green-500: #34a853;
	--glue-green-600: #1e8e3e;
	--glue-green-700: #188038;
	--glue-green-800: #137333;
	--glue-green-900: #0d652d;
	--glue-red-50: #fce8e6;
	--glue-red-100: #fad2cf;
	--glue-red-200: #f6aea9;
	--glue-red-300: #f28b82;
	--glue-red-400: #ee675c;
	--glue-red-500: #ea4335;
	--glue-red-600: #d93025;
	--glue-red-700: #c5221f;
	--glue-red-800: #b31412;
	--glue-red-900: #a50e0e;
	--glue-yellow-50: #fef7e0;
	--glue-yellow-100: #feefc3;
	--glue-yellow-200: #fde293;
	--glue-yellow-300: #fdd663;
	--glue-yellow-400: #fcc934;
	--glue-yellow-500: #fbbc04;
	--glue-yellow-600: #f9ab00;
	--glue-yellow-700: #f29900;
	--glue-yellow-800: #ea8600;
	--glue-yellow-900: #e37400;
	--glue-purple-100: #ea80fc;
	--glue-purple-900: #681da8;
}
```

## Themes

```css
/* @tailwind base;
@tailwind components;
@tailwind utilities; */

@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300..800;1,300..800&display=swap');
@import url('https://fonts.googleapis.com/css2?family=JetBrains+Mono:ital,wght@0,100..800;1,100..800&display=swap');

/* color mode default settings */
:root {
	color-scheme: light;
	--bg-primary: #fff;
	--bg-secondary: #fcfcfc;
	--bg-third: #fafafa;
	--text-primary: #0d0d0d;
	--text-secondary: #73747a;
	--text-third: #5f6368;
	--accent-primary: #6dd338;
	--accent-secondary: #71e935;
	--accent-third: #a6ff79;
	--divider-primary: #dadce0;
	--border-primary: #d8dad5;
	--placeholder: #ddd;
	--logo: url('/default/logo/logo-light.png');
}

/* color mode from browser settings */
@media (prefers-color-scheme: dark) {
	:root {
		color-scheme: dark;
		--bg-primary: #202331;
		--bg-secondary: #232634;
		--bg-third: #262a3a;
		--text-primary: #fff;
		--text-secondary: #9da2b9;
		--text-third: #666c88;
		--accent-primary: #6dd338;
		--placeholder: #2d3145;
		--code-border: #2d3145;
		--divider-primary: #2d3145;
		--border-primary: #2d3145;
		--logo: url('/default/logo/logo-dark.png');
		--input-background-color: var(--bg-third);
		--input-border-color: var(--border-primary);
		--input-label-color: var(--text-third);
	}
}

/* color mode from html tag attribute */
[color-scheme='light'] {
	color-scheme: light;
	--bg-primary: #fff;
	--bg-secondary: #fcfcfc;
	--bg-third: #fafafa;
	--text-primary: #0d0d0d;
	--text-secondary: #73747a;
	--text-third: #5f6368;
	--accent-primary: #6dd338;
	--accent-secondary: #71e935;
	--divider-primary: #dadce0;
	--border-primary: #d8dad5;
	--placeholder: #ddd;
	--logo: url('/default/logo/logo-light.png');
}

[color-scheme='dark'] {
	color-scheme: dark;
	--bg-primary: #202331;
	--bg-secondary: #232634;
	--bg-third: #262a3a;
	--text-primary: #fff;
	--text-secondary: #9da2b9;
	--text-third: #666c88;
	--accent-primary: #6dd338;
	--accent-secondary: #71e935;
	--placeholder: #2d3145;
	--code-border: #2d3145;
	--divider-primary: #2d3145;
	--border-primary: #2d3145;
	--logo: url('/default/logo/logo-dark.png');
	--input-background-color: var(--bg-third);
	--input-border-color: var(--border-primary);
	--input-label-color: var(--text-third);
}

:root {
	/* page */
	--font-family: 'Poppins', Arial, Helvetica, sans-serif;
	--font-family-code: 'JetBrains Mono', 'Fira Code', monospace;
	--font-size: 16px;
	--border-radius: 6px;
	--button-border-radius: 10px;

	/* scrollbar */
	--scrollbar-width: 10px;
	--scrollbar-bg-thin: #e6e6e6;
	--scrollbar-thumb-thin: #6dd338;

	/* form inputs */
	--input-border-radius: 10px;
	--input-background-color: var(--bg-third);
	--input-border-color: var(--border-primary);
	--input-label-color: var(--text-third);

	/* input alerts */
	--input-alert-error: #fe093a;
	--input-alert-error-bg: linear-gradient(
		to right,
		#fe093a15,
		#fe093a06
	);
	--input-alert-info: #00b13f;
	--input-alert-info-bg: linear-gradient(
		to right,
		#00b13f15,
		#00b13f06
	);
}

* {
	outline: 0px none transparent;
	box-sizing: border-box;
	text-decoration: none;
}

::before,
::after {
	box-sizing: border-box;
	content: none;
}

::placeholder {
	color: var(--placeholder);
	opacity: 1;
}

::selection {
	background: #0e7aff;
	color: #fff;
}

#app {
	overflow: hidden;
	padding: 0px;
	margin: 0px;
}

html,
body {
	margin: 0px;
	padding: 0px;
	min-height: 100vh;
	font-size: var(--font-size);
	font-family: var(--font-family);
	background: var(--bg-primary);
	transition: all 0.5s;
}

html {
	overflow-y: scroll;
}

iframe {
	color-scheme: light !important;
}

p {
	font-family: var(--font-family);
}

img,
svg {
	display: inline-block;
	max-width: 100%;
}

/* panel scrollbar */
.scrollbar-thin {
	scrollbar-width: thin;
	scrollbar-color: var(--scrollbar-thumb-thin)
		var(--scrollbar-bg-thin);
}

.scrollbar-thin::-webkit-scrollbar {
	width: var(--scrollbar-width);
	background: var(--scrollbar-thumb-thin);
}

.scrollbar-thin::-webkit-scrollbar-thumb {
	background: var(--scrollbar-bg-thin);
}

/* page sections */
.section {
	float: left;
	width: 100%;
	min-height: 100vh;
	position: relative;
}

.section-center {
	margin: 0px auto;
	height: auto;
	width: 90%;
	max-width: 1120px;
}
```

## Load svg vue3 component

```vue
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
```
