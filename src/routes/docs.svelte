<script context="module">
	import { browser, dev } from '$app/env';

	// we don't need any JS on this page, though we'll load
	// it in dev so that we get hot module replacement...
	export const hydrate = dev;

	// ...but if the client-side router is already loaded
	// (i.e. we came here from elsewhere in the app), use it
	export const router = browser;

	// since there's no dynamic data here, we can prerender
	// it so that it gets served as a static asset in prod
	export const prerender = true;
</script>

<svelte:head>
	<title>Docs</title>
</svelte:head>

<section>
	<h1>Docs</h1>

	<h2>Heading</h2>
	<!-- codesandbox -->

	<!-- codesandbox -->
	<h2>Color</h2>
	<h3>Main Color</h3>
	<h3>Text Color</h3>
	<h3>Desc Color</h3>
	<h3>Disabled Color</h3>
	<h3>Icon Color</h3>
	<!-- codesandbox -->

	<!-- codesandbox -->

	<h2>Font Size</h2>

	<h2>Heading</h2>
	<h3>Heading Icon Color Variation</h3>
	<h3>Heading Title Icon Sizes</h3>
	<h3>Heading1 Title Icon Sizes (+Icon-only version)</h3>
	<h3>Heading1 Title Icon (+Text) </h3>
	<h3>Heading1 Title Icon (+Text) (+Single) </h3>
	<h3>Heading1 Title Icon (+Text) (+Single) </h3>
	<h3>Heading1 Title Icon (+Text) (+Desc)</h3>
	<h3>Heading1 Title Icon (+Text) (+Desc)</h3>

	<h2>Button</h2>
	<h3>Normal</h3>
	<h3>Rounded</h3>
</section>

<style>
	section {
		padding: 0 32px;
	}
	.black-icon {
		color: #000;
	}
	.yellow {
		background-color: #FCCC0A;
	}
</style>
