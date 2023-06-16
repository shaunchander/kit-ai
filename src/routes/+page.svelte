<script lang="ts">
	import Container from '$lib/components/Container.svelte';
	import Section from '$lib/components/Section.svelte';
	import { Button } from '$lib/components/ui/button';
	import { CheckCircleIcon } from 'svelte-feather-icons';
</script>

<Section id="hero" className="relative pt-24 md:pt-40">
	<Container className="space-y-6">
		<div class="md:text-center space-y-4">
			<h1>
				Batteries-included AI templates for <span
					class="inline-flex animate-background-shine bg-[linear-gradient(110deg,#cbd5e1,45%,#6366f1,55%,#cbd5e1)] bg-[length:250%_100%] bg-clip-text text-transparent"
					>SvelteKit</span
				>
				and
				<span
					class="inline-flex animate-background-shine bg-[linear-gradient(110deg,#cbd5e1,45%,#6366f1,55%,#cbd5e1)] bg-[length:250%_100%] bg-clip-text text-transparent"
					>Next.js</span
				>.
			</h1>
			<p class="text-lg text-slate-500 font-medium">🚀 Launch that AI project sooner with KitAI.</p>
			<div>
				<Button>Pre-order at &nbsp;<s class="text-sm text-slate-600">$49</s>&nbsp; $29</Button>
			</div>
		</div>
		<div>
			<ul class="grid grid-cols-2 gap-4 md:grid-cols-3 md:justify-items-center">
				<li class="flex gap-x-2">
					<div>
						<CheckCircleIcon class="text-green-600 w-4 h-4" />
					</div>
					<p
						class="text-sm text-clip bg-gradient-to-t from-slate-800 to-slate-50 text-transparent bg-clip-text"
					>
						Vercel AI SDK integration
					</p>
				</li>
				<li class="flex gap-x-2">
					<div>
						<CheckCircleIcon class="text-green-600 w-4 h-4" />
					</div>
					<p
						class="text-sm text-clip bg-gradient-to-t from-slate-800 to-slate-50 text-transparent bg-clip-text"
					>
						LemonSqueezy payments integration
					</p>
				</li>
				<li class="flex gap-x-2">
					<div>
						<CheckCircleIcon class="text-green-600 w-4 h-4" />
					</div>
					<p
						class="text-sm text-clip bg-gradient-to-t from-slate-800 to-slate-50 text-transparent bg-clip-text"
					>
						Supabase integration
					</p>
				</li>
				<li class="flex gap-x-2">
					<div>
						<CheckCircleIcon class="text-green-600 w-4 h-4" />
					</div>
					<p
						class="text-sm text-clip bg-gradient-to-t from-slate-800 to-slate-50 text-transparent bg-clip-text"
					>
						User accounts and settings
					</p>
				</li>
				<li class="flex gap-x-2">
					<div>
						<CheckCircleIcon class="text-green-600 w-4 h-4" />
					</div>
					<p
						class="text-sm text-clip bg-gradient-to-t from-slate-800 to-slate-50 text-transparent bg-clip-text"
					>
						License-based usage
					</p>
				</li>
				<li class="flex gap-x-2">
					<div>
						<CheckCircleIcon class="text-green-600 w-4 h-4" />
					</div>
					<p
						class="text-sm text-clip bg-gradient-to-t from-slate-800 to-slate-50 text-transparent bg-clip-text"
					>
						Landing page
					</p>
				</li>
			</ul>
		</div>
	</Container>
	<img
		src="/bg.png"
		alt=""
		class="absolute inset-0 h-full w-full object-cover opacity-50 pointer-events-none"
	/>
</Section>
