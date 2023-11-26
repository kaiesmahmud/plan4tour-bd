<script lang="ts">
	import { Accordion as AccordionPrimitive } from "bits-ui";
	import { cn } from "$lib/utils";
	import { slide } from "svelte/transition";

	type $$Props = AccordionPrimitive.ContentProps;

	let className: $$Props["class"] = undefined;
	export let transition: $$Props["transition"] = slide;
	export let transitionConfig: $$Props["transitionConfig"] = {
		duration: 200
	};
	export { className as class };
</script>

<AccordionPrimitive.Content
	class={cn("overflow-hidden transition-all text-lg lg:text-xl text-white/90 p-3 font-light", className)}
	{transition}
	{transitionConfig}
	{...$$restProps}
>
	<div class="pb-4 pt-0">
		<slot />
	</div>
</AccordionPrimitive.Content>
