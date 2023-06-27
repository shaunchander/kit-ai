<script>
	import Container from '$lib/components/Container.svelte';
</script>

<footer class="p-6">
	<Container className="space-y-4 md:flex md:justify-between md:items-center">
		<div class="w-full absolute top-0 inset-x-0 h-px bg-slate-800 -mt-4" />

		<div class="space-y-1 mt-4">
			<p>
				<span class="text-slate-300 text-xl">KitAI</span>
			</p>
			<p class="text-slate-500 text-sm">
				Built and maintained by <a
					class="font-medium text-slate-400 hover:text-slate-300 duration-300 ease-in-out"
					href="https://twitter.com/shaunchander"
					target="_blank">Shaun Chander</a
				>.
			</p>
		</div>
		<div>
			<ul class="flex items-center gap-x-2">
				<li>
					<a
						class="text-slate-400 text-sm hover:text-slate-300 duration-300 ease-in-out"
						href="/privacy-policy">Privacy Policy</a
					>
				</li>
				<li>
					<a
						class="text-slate-400 text-sm hover:text-slate-300 duration-300 ease-in-out"
						href="mailto:kitai@shaunchander.me">Contact</a
					>
				</li>
			</ul>
		</div>
	</Container>
</footer>
