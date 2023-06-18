<script lang="ts">
	import { cn } from '$lib/utils';

	export let id: string;
	export let className = '';
</script>

<section {id} class={cn('p-6 md:p-10 py-12 md:py-20', className)}><slot /></section>
