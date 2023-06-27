<script lang="ts">
	import { cn } from '$lib/utils';

	export let className = '';
</script>

<div class={cn('container mx-auto max-w-4xl', className)}><slot /></div>
