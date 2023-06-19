<script lang="ts">
	import '../switzer.css';
	import '../app.postcss';
	import Header from '$components/Header.svelte';
	import Footer from '$components/Footer.svelte';
	import { Somerset } from 'somerset';
	import { dev } from '$app/environment';
</script>

<svelte:head>
	<link rel="apple-touch-icon" sizes="57x57" href="/favicons/favicon-57x57.png" />
	<link rel="apple-touch-icon" sizes="60x60" href="/favicons/favicon-60x60.png" />
	<link rel="apple-touch-icon" sizes="72x72" href="/favicons/favicon-72x72.png" />
	<link rel="apple-touch-icon" sizes="76x76" href="/favicons/favicon-76x76.png" />
	<link rel="apple-touch-icon" sizes="114x114" href="/favicons/favicon-114x114.png" />
	<link rel="apple-touch-icon" sizes="120x120" href="/favicons/favicon-120x120.png" />
	<link rel="apple-touch-icon" sizes="144x144" href="/favicons/favicon-144x144.png" />
	<link rel="apple-touch-icon" sizes="152x152" href="/favicons/favicon-152x152.png" />
	<link rel="apple-touch-icon" sizes="180x180" href="/favicons/favicon-180x180.png" />
	<link rel="icon" type="image/png" sizes="16x16" href="/favicons/favicon-16x16.png" />
	<link rel="icon" type="image/png" sizes="32x32" href="/favicons/favicon-32x32.png" />
	<link rel="icon" type="image/png" sizes="96x96" href="/favicons/favicon-96x96.png" />
	<link rel="icon" type="image/png" sizes="192x192" href="/favicons/favicon-192x192.png" />
	<link rel="shortcut icon" type="image/x-icon" href="/favicons/favicon.ico" />
	<link rel="icon" type="image/x-icon" href="/favicons/favicon.ico" />
	<meta name="msapplication-TileColor" content="#020617" />
	<meta name="msapplication-TileImage" content="/favicons/favicon-144x144.png" />
	<meta name="msapplication-config" content="/browserconfig.xml" />

	{#if !dev}
		<script
			async
			src="https://umami.services.shaunchander.me/script.js"
			data-website-id="2a1a6997-3061-4330-bb18-0598f013d5d7"
		></script>
	{/if}
</svelte:head>

<Somerset
	title="KitAI"
	description="Get started on your AI project sooner with our batteries-included AI templates for SvelteKit and NextJS. Our templates leverage Vercel's AI SDK, LemonSqueezy checkouts, and Supabase!"
	openGraph={{
		title: 'KitAI',
		description:
			"Get started on your AI project sooner with our batteries-included AI templates for SvelteKit and NextJS. Our templates leverage Vercel's AI SDK, LemonSqueezy checkouts, and Supabase!",
		siteName: 'KitAI',
		images: [
			{
				url: 'https://',
				alt: ''
			}
		]
	}}
	twitter={{
		cardType: 'summary_large_image'
	}}
/>

<div class="min-h-screen flex flex-col bg-slate-950 font-body text-slate-50 relative">
	<Header />
	<main class="flex flex-1 flex-col">
		<slot />
	</main>
	<Footer />
</div>
