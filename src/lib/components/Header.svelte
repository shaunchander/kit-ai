<script>
	import { PUBLIC_LEMONSQUEEZY_CHECKOUT } from '$env/static/public';
	import Container from './Container.svelte';
</script>

<header class="inset-x-0 top-0 p-6 fixed backdrop-blur-sm z-50">
	<nav>
		<Container>
			<div class="flex items-center justify-between">
				<div>
					<a href="/" class="flex items-center justify-center text-sm font-medium">
						<span
							class="bg-gradient-to-t from-slate-100 to-indigo-500 bg-clip-text text-xl text-transparent md:text-2xl"
							>KitAI</span
						>
					</a>
				</div>
				<div>
					<a
						href={PUBLIC_LEMONSQUEEZY_CHECKOUT}
						class="relative inline-flex h-12 overflow-hidden rounded-full p-[1px] focus:outline-none focus:ring-2 focus:ring-slate-400 focus:ring-offset-2 focus:ring-offset-slate-50"
					>
						<span
							class="absolute inset-[-1000%] animate-[spin_2s_linear_infinite] bg-[conic-gradient(from_90deg_at_50%_50%,#64748b_0%,#6366f1_50%,#E2CBFF_100%)]"
						/>
						<span
							class="inline-flex h-full w-full cursor-pointer items-center justify-center rounded-full bg-slate-900 px-6 py-1 text-sm font-medium text-white backdrop-blur-3xl"
						>
							Pre-order
						</span>
					</a>
				</div>
			</div>
		</Container>
	</nav>
</header>
