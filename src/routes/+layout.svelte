<script lang="ts">
	import '../switzer.css';
	import '../app.postcss';
	import Header from '$components/Header.svelte';
</script>

<div class="min-h-screen flex flex-col bg-slate-950 font-body text-slate-50">
	<Header />
	<main>
		<slot />
	</main>
</div>
