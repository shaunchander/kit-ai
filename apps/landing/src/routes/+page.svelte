<script lang="ts">
	import Plyr from 'plyr';
	import {
		Accordion,
		AccordionContent,
		AccordionItem,
		AccordionTrigger
	} from '$components/ui/accordion';
	import Badge from '$components/ui/badge/Badge.svelte';

	import {
		DialogTrigger,
		Dialog,
		DialogHeader,
		DialogTitle,
		DialogDescription,
		DialogContent
	} from '$components/ui/dialog';
	import { PUBLIC_LEMONSQUEEZY_CHECKOUT } from '$env/static/public';
	import Container from '$lib/components/Container.svelte';
	import Section from '$lib/components/Section.svelte';
	import { Button } from '$lib/components/ui/button';
	import { CheckCircleIcon } from 'svelte-feather-icons';
	import { Input } from '$components/ui/input';
</script>

<Section
	id="hero"
	className="relative pt-24 md:pt-0 pb-20 md:pb-24 md:min-h-[500px] md:h-[75svh] md:flex md:items-center"
>
	<Container className="space-y-8">
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
			<p class="text-lg text-slate-400 font-medium">Launch that AI SaaS sooner with KitAI.</p>
			<div>
				<Button href={PUBLIC_LEMONSQUEEZY_CHECKOUT}
					>Pre-order at &nbsp;<s class="text-sm text-slate-600">$49</s>&nbsp; $29</Button
				>
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
						LemonSqueezy checkouts
					</p>
				</li>
				<li class="flex gap-x-2">
					<div>
						<CheckCircleIcon class="text-green-600 w-4 h-4" />
					</div>
					<p
						class="text-sm text-clip bg-gradient-to-t from-slate-800 to-slate-50 text-transparent bg-clip-text"
					>
						Supabase-powered backend
					</p>
				</li>
				<li class="flex gap-x-2">
					<div>
						<CheckCircleIcon class="text-green-600 w-4 h-4" />
					</div>
					<p
						class="text-sm text-clip bg-gradient-to-t from-slate-800 to-slate-50 text-transparent bg-clip-text"
					>
						User dashboards and settings
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
						Beatifully designed landing page
					</p>
				</li>
			</ul>
		</div>
	</Container>

	<img
		src="/bg.png"
		alt=""
		class="absolute top-0 left-0 h-full w-full object-cover opacity-50 pointer-events-none"
	/>
	<div
		class="bg-gradient-to-t from-slate-950 to-transparent absolute bottom-0 pointer-events-none inset-x-0 h-12"
	/>
</Section>

<Section id="setting-up-kitai">
	<Container className="space-y-10">
		<div class="text-center">
			<h2 class="bg-gradient-to-tl from-slate-900 to-slate-50 bg-clip-text text-transparent">
				Available templates
			</h2>
		</div>
		<ul class="grid md:grid-cols-3">
			<li>
				<Dialog>
					<DialogTrigger>
						<div
							class="rounded-2xl border border-slate-800 divide-y divide-slate-800 hover:shadow-xl hover:shadow-slate-200/5 transition duration-300 ease-in-out"
						>
							<div class="relative h-48 overflow-hidden">
								<div class="absolute top-2 right-2">
									<Badge>Pre-order</Badge>
								</div>
								<img
									src="/chat-preview.svg"
									class="w-1/2 select-none mx-auto h-full transform translate-y-1"
									alt=""
								/>
							</div>
							<div class="p-4 text-left">
								<h3 class="text-slate-200">Chat KitAI <span /></h3>
								<p class="text-slate-400">
									Build and launch chat-powered AI applications with ease.
								</p>
							</div>
						</div>
					</DialogTrigger>
					<DialogContent class="border-slate-800 bg-slate-950">
						<div class="mt-8 lg:flex lg:gap-x-12">
							<div class="w-full relative">
								<video class="rounded-sm w-full" autoplay loop>
									<source src="/chat-kitai-demo.mp4" type="video/mp4" />

									Your browser does not support HTML video.
								</video>
								<div class="absolute top-2 right-2">
									<Badge>Early concept design</Badge>
								</div>
							</div>
							<div class="mt-6 lg:mt-0">
								<DialogHeader>
									<DialogTitle class="text-slate-50 text-left">Chat KitAI</DialogTitle>
									<DialogDescription class="text-slate-300 text-left">
										Build chat-enabled AI apps with Vercel's AI SDK and OpenAI.
									</DialogDescription>
								</DialogHeader>
								<div class="mt-6 space-y-8">
									<div>
										<ul class="grid grid-cols-2 gap-4 md:grid-cols-2">
											<li class="flex gap-x-2">
												<div>
													<CheckCircleIcon class="text-green-600 w-4 h-4" />
												</div>
												<p class="text-sm text-slate-400">Vercel AI SDK</p>
											</li>
											<li class="flex gap-x-2">
												<div>
													<CheckCircleIcon class="text-green-600 w-4 h-4" />
												</div>
												<p class="text-sm text-slate-400">OpenAI integration</p>
											</li>
											<li class="flex gap-x-2">
												<div>
													<CheckCircleIcon class="text-green-600 w-4 h-4" />
												</div>
												<p class="text-sm text-slate-400">LemonSqueezy checkout</p>
											</li>
											<li class="flex gap-x-2">
												<div>
													<CheckCircleIcon class="text-green-600 w-4 h-4" />
												</div>
												<p class="text-sm text-slate-400">Supabase-powered backend</p>
											</li>
											<li class="flex gap-x-2">
												<div>
													<CheckCircleIcon class="text-green-600 w-4 h-4" />
												</div>
												<p class="text-sm text-slate-400">
													User accounts, dashboards, and settings
												</p>
											</li>
											<li class="flex gap-x-2">
												<div>
													<CheckCircleIcon class="text-green-600 w-4 h-4" />
												</div>
												<p class="text-sm text-slate-400">Includes landing page and chat page</p>
											</li>
											<li class="flex gap-x-2">
												<div>
													<CheckCircleIcon class="text-green-600 w-4 h-4" />
												</div>
												<p class="text-sm text-slate-400">Built with Stream API</p>
											</li>
											<li class="flex gap-x-2">
												<div>
													<CheckCircleIcon class="text-green-600 w-4 h-4" />
												</div>
												<p class="text-sm text-slate-400">Full asset ownership</p>
											</li>
										</ul>
									</div>
									<Button href={PUBLIC_LEMONSQUEEZY_CHECKOUT} class="w-full"
										>Pre-order at&nbsp;<s class="text-slate-600">$49</s> &nbsp; $29</Button
									>
								</div>
							</div>
						</div>
					</DialogContent>
				</Dialog>
			</li>
		</ul>
		<div class="space-y-4 md:max-w-md md:mx-auto">
			<div class="space-y-2">
				<h3 class="text-slate-300">Stay up to date with KitAI?</h3>
				<p class="text-sm text-slate-500">
					We don't spam. We'll just send you updates on KitAI if you wanna keep a watchful eye!
				</p>
			</div>
			<form action="https://kitai.lemonsqueezy.com/email-subscribe/external" method="POST">
				<Input
					type="email"
					class="border-slate-800"
					name="email"
					placeholder="Enter your email..."
					required
				/>
			</form>
		</div>
	</Container>
</Section>

<Section id="faq">
	<Container>
		<div class="relative md:grid md:grid-cols-2 md:gap-x-10">
			<div class="space-y-2 md:sticky md:top-[100px]">
				<h2 class="bg-gradient-to-tl from-slate-900 to-slate-50 bg-clip-text text-transparent">
					Frequently Asked Questions
				</h2>
				<p class="text-slate-500 font-medium">
					Want to ask a specific question? <a
						href="mailto:kitai@shaunchander.me"
						class="text-slate-400 hover:text-slate-300 duration-300 ease-in-out"
						>Send us an email!</a
					> We'll get back to you within a day.
				</p>
			</div>
			<Accordion type="single" collapsible class="text-slate-300">
				<AccordionItem value="item-1" class="border-slate-800">
					<AccordionTrigger>When will KitAI be available?</AccordionTrigger>
					<AccordionContent
						>I'm aiming to have Chat KitAI (our first template) out and ready for prod by the middle
						of July.</AccordionContent
					>
				</AccordionItem>
				<AccordionItem value="item-2" class="border-slate-800">
					<AccordionTrigger class="text-left"
						>Will KitAI recieve updates post-purchase?</AccordionTrigger
					>
					<AccordionContent
						>KitAI templates will recieve quality-of-life updates as needed! This includes QOL
						updates for both our Next.js and SvelteKit template versions and QOL updates that cover
						any major API updates from our integrations: LemonSqueezy, Supabase, Vercel AI SDK.</AccordionContent
					>
				</AccordionItem>
				<AccordionItem value="item-3" class="border-slate-800">
					<AccordionTrigger>How can I customize KitAI?</AccordionTrigger>
					<AccordionContent
						>While we ship a fully end-to-end integrated templates that can be hosted immedietly,
						you can control and modify as much of KitAI as you want. You will need to know your way
						around SvelteKit/Next.js in order to make changes. Remember, KitAI is a template with
						suggessted defaults and integrations. You can use as much or as little of KitAI as you'd
						like in your project!</AccordionContent
					>
				</AccordionItem>
				<AccordionItem value="item-4" class="border-slate-800">
					<AccordionTrigger>Is there a refund policy?</AccordionTrigger>
					<AccordionContent
						>Yes! You'll have up to 30 days after purchase to recieve a full refund. In the meantime
						if you have any questions or need support reach out to us over email!</AccordionContent
					>
				</AccordionItem>
			</Accordion>
		</div>
	</Container>
</Section>
