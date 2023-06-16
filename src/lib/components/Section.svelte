<script lang="ts">
	import { cn } from '$lib/utils';

	export let id: string;
	export let className = '';
</script>

<section {id} class={cn('p-6 md:p-10', className)}><slot /></section>
