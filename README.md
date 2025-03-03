# Css dark mode theme
Css styles ...

## Import

```css
@import url('@/assets/css/root.css');
```

## Black white theme 

```
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300..800;1,300..800&display=swap');
@import url('https://fonts.googleapis.com/css2?family=JetBrains+Mono:ital,wght@0,100..800;1,100..800&display=swap');

:root {
	/* White */
	--w-accent-1: #0075ff;
	--w-accent-2: #0045cc;
	--w-accent-3: #0075ff11;
	--w-bg-1: #ffffff;
	--w-bg-2: #fbfbfb;
	--w-bg-3: #f3f3f3;
	--w-text-1: #0a0a0a;
	--w-text-2: #909090;
	--w-text-3: #b0b0b0;
	--w-border: #e5e5e5; /* #cccecd */
	--w-holder: #969696;
	--b-disabled: #999999;
	--w-scroll-bg: #f5f5f5;
	--w-scroll-th: #dcdcdc;
	--w-label: #707070;
	--w-input: #fcfcfc;
	--w-icon: #cccccc;
	--w-red: #cd3310;
	--w-green: #258c60;
	--w-selection: #ffffff;
	--w-selection-bg: #0e7aff;
	--w-alert: #ff303c;

	/* Black */
	--b-accent-1: #0075ff;
	--b-accent-2: #0045cc;
	--w-accent-3: #0075ff11;
	--b-bg-1: #1c1c1c;
	--b-bg-2: #1f1f1f;
	--b-bg-3: #f7f7f7;
	--b-text-1: #e8e8e8;
	--b-text-2: #7e7e7e;
	--b-text-3: #797979;
	--b-border: #2c2c2c;
	--b-holder: #969696;
	--b-disabled: #999999;
	--b-scroll-bg: #242424;
	--b-scroll-th: #3a3a3a;
	--b-label: #606060;
	--b-input: #1f1f1f;
	--b-icon: #4c4c4c;
	--b-red: #cd3310;
	--b-green: #258c60;
	--b-selection: #ffffff;
	--b-selection-bg: #0e7aff;
	--b-alert: #ff303c;
}

:root {
	color-scheme: light;
	--bg-1: var(--w-bg-1);
	--bg-2: var(--w-bg-2);
	--bg-3: var(--w-bg-3);
	--text-1: var(--w-text-1);
	--text-2: var(--w-text-2);
	--text-3: var(--w-text-3);
	--icon-1: var(--w-icon);
	--icon-2: var(--w-icon);
	--icon-3: var(--w-icon);
	--accent: var(--w-accent-1);
	--accent-hover: var(--w-accent-2);
	--disabled: var(--w-disabled);
	--border: var(--w-border);
	--divider: var(--w-border);
	--placeholder: var(--w-holder);
	--selection-color: var(--w-selection);
	--selection-bg: var(--w-selection-bg);
	--scrollbar-bg: var(--w-scroll-bg);
	--scrollbar-thumb: var(--w-scroll-th);
	--scrollbar-width: 8px;
	--logo: url('/default/logo/logo-light.png');
	--input-font-family: var(--font-family);
	--input-radius: 10px;
	--input-font-size: 16px;
	--input-icon: var(--w-icon);
	--input-holder: var(--w-holder);
	--input-label: var(--w-label);
	--input-border: var(--w-border);
	--input-shadow: var(--w-accent-3);
	--input-bg: var(--w-input);
	--column: var(--w-label);
	--button-bg: var(--w-accent-1);
	--button-color: var(--w-text-1);
	--button-border: var(--w-accent-2);
	--button-radius: 10px;
	--alert: var(--w-alert);
}

/* color mode from browser settings */
@media (prefers-color-scheme: dark) {
	:root {
		color-scheme: dark;
		--bg-1: var(--b-bg-1);
		--bg-2: var(--b-bg-2);
		--bg-3: var(--b-bg-3);
		--text-1: var(--b-text-1);
		--text-2: var(--b-text-2);
		--text-3: var(--b-text-3);
		--icon-1: var(--b-icon);
		--icon-2: var(--b-icon);
		--icon-3: var(--b-icon);
		--accent: var(--b-accent-1);
		--accent-hover: var(--b-accent-2);
		--disabled: var(--b-disabled);
		--border: var(--b-border);
		--divider: var(--b-border);
		--placeholder: var(--b-holder);
		--selection-color: var(--b-selection);
		--selection-bg: var(--b-selection-bg);
		--scrollbar-bg: var(--b-scroll-bg);
		--scrollbar-thumb: var(--b-scroll-th);
		--scrollbar-width: 8px;
		--logo: url('/default/logo/logo-dark.png');
		--input-font-family: var(--font-family);
		--input-radius: 10px;
		--input-font-size: 16px;
		--input-icon: var(--b-icon);
		--input-holder: var(--b-holder);
		--input-label: var(--b-label);
		--input-border: var(--b-border);
		--input-shadow: var(--b-accent-3);
		--input-bg: var(--b-input);
		--column: var(--b-label);
		--button-bg: var(--b-accent-1);
		--button-color: var(--b-text-1);
		--button-border: var(--b-accent-2);
		--button-radius: 10px;
		--alert: var(--b-alert);
	}
}

/* color mode from <html color-scheme="light"> */
[color-scheme='light'] {
	color-scheme: light;
	--bg-1: var(--w-bg-1);
	--bg-2: var(--w-bg-2);
	--bg-3: var(--w-bg-3);
	--text-1: var(--w-text-1);
	--text-2: var(--w-text-2);
	--text-3: var(--w-text-3);
	--icon-1: var(--w-icon);
	--icon-2: var(--w-icon);
	--icon-3: var(--w-icon);
	--accent: var(--w-accent-1);
	--accent-hover: var(--w-accent-2);
	--disabled: var(--w-disabled);
	--border: var(--w-border);
	--divider: var(--w-border);
	--placeholder: var(--w-holder);
	--selection-color: var(--w-selection);
	--selection-bg: var(--w-selection-bg);
	--scrollbar-bg: var(--w-scroll-bg);
	--scrollbar-thumb: var(--w-scroll-th);
	--scrollbar-width: 8px;
	--logo: url('/default/logo/logo-light.png');
	--input-font-family: var(--font-family);
	--input-radius: 10px;
	--input-font-size: 16px;
	--input-icon: var(--w-icon);
	--input-holder: var(--w-holder);
	--input-label: var(--w-label);
	--input-border: var(--w-border);
	--input-shadow: var(--w-accent-3);
	--input-bg: var(--w-input);
	--column: var(--w-label);
	--button-bg: var(--w-accent-1);
	--button-color: var(--w-text-1);
	--button-border: var(--w-accent-2);
	--button-radius: 10px;
	--alert: var(--w-alert);
}

/* color mode from <html color-scheme="dark"> */
[color-scheme='dark'] {
	color-scheme: dark;
	--bg-1: var(--b-bg-1);
	--bg-2: var(--b-bg-2);
	--bg-3: var(--b-bg-3);
	--text-1: var(--b-text-1);
	--text-2: var(--b-text-2);
	--text-3: var(--b-text-3);
	--icon-1: var(--b-icon);
	--icon-2: var(--b-icon);
	--icon-3: var(--b-icon);
	--accent: var(--b-accent-1);
	--accent-hover: var(--b-accent-2);
	--disabled: var(--b-disabled);
	--border: var(--b-border);
	--divider: var(--b-border);
	--placeholder: var(--b-holder);
	--selection-color: var(--b-selection);
	--selection-bg: var(--b-selection-bg);
	--scrollbar-bg: var(--b-scroll-bg);
	--scrollbar-thumb: var(--b-scroll-th);
	--scrollbar-width: 8px;
	--logo: url('/default/logo/logo-dark.png');
	--input-font-family: var(--font-family);
	--input-radius: 10px;
	--input-font-size: 16px;
	--input-icon: var(--b-icon);
	--input-holder: var(--b-holder);
	--input-label: var(--b-label);
	--input-border: var(--b-border);
	--input-shadow: var(--b-accent-3);
	--input-bg: var(--b-input);
	--column: var(--b-label);
	--button-bg: var(--b-accent-1);
	--button-color: var(--b-text-1);
	--button-border: var(--b-accent-2);
	--button-radius: 10px;
	--alert: var(--b-alert);
}

/* page */
:root {
	--font-family: 'Poppins', Arial, Helvetica, sans-serif;
	--font-family-code: 'JetBrains Mono', 'Fira Code', monospace;
	--font-size: 16px;
	--border-radius: 6px;
	--button-border-radius: 10px;
	--gap: 20px;

	/* alert error */
	--alert-error: #fe093a;
	--alert-error-bg: linear-gradient(to right, #fe093a15, #fe093a06);

	/* alert ok */
	--alert-info: #00b13f;
	--alert-info-bg: linear-gradient(to right, #00b13f15, #00b13f06);
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
	color: var(--placeholder-1);
	opacity: 1;
}

::selection {
	background: var(--selection-bg);
	color: var(--selection-color);
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
	background: var(--bg-1);
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
	scrollbar-color: var(--w-accent-1) var(--scrollbar-bg);
}

.scrollbar-thin::-webkit-scrollbar {
	width: var(--scrollbar-width);
	background: var(--w-accent-1);
}

.scrollbar-thin::-webkit-scrollbar-thumb {
	background: var(--scrollbar-bg);
}

/* navbar scrollbar */
.scrollbar-navbar {
	scrollbar-width: thin;
	scrollbar-color: var(--scrollbar-thumb) var(--scrollbar-bg);
}

.scrollbar-navbar::-webkit-scrollbar {
	width: var(--scrollbar-width);
	background: var(--scrollbar-thumb);
}

.scrollbar-navbar::-webkit-scrollbar-thumb {
	background: var(--scrollbar-bg);
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

/* logo */
img.logo {
	content: var(--logo);
}
```
