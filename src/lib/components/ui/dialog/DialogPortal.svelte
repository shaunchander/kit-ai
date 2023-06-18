<script lang="ts">
	import { Dialog as DialogPrimitive } from 'radix-svelte';
</script>

<DialogPrimitive.Portal>
	<div class="fixed inset-0 z-50 flex items-center justify-center">
		<slot />
	</div>
</DialogPrimitive.Portal>
