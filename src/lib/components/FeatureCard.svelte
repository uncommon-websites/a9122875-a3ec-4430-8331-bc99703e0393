<script lang="ts">
	export let tagColor: string = "bg-brand-primary";
	export let tagIcon: string = "arrow"; // arrow or plus
	export let title: string;
	export let subtitle: string; // Small red text above title
	export let description: string;
	export let imageSrc: string = "";
</script>

<div class="bg-[#F3F3F1] rounded-lg p-8 relative overflow-hidden flex flex-col h-full border border-gray-200 shadow-sm hover:shadow-md transition-shadow">
	<div class="absolute top-4 right-4 w-6 h-6 {tagColor} text-white flex items-center justify-center rounded-sm z-10">
		{#if tagIcon === 'arrow'}
			<svg xmlns="http://www.w3.org/2000/svg" width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="3" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14"/><path d="m12 5 7 7-7 7"/></svg>
		{:else}
			<svg xmlns="http://www.w3.org/2000/svg" width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="3" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14"/><path d="M12 5v14"/></svg>
		{/if}
	</div>

	<div class="mb-6 z-10 relative">
		<span class="font-mono text-[10px] text-accent-pink uppercase tracking-widest mb-2 block">
			{subtitle}
		</span>
		<h3 class="font-display text-2xl md:text-3xl font-medium leading-tight mb-4 tracking-tight">
			{@html title}
		</h3>
		<p class="text-sm text-gray-600 leading-relaxed max-w-sm">
			{description}
		</p>
	</div>

	<div class="mt-auto relative w-full aspect-[4/3] bg-white rounded border border-gray-200 shadow-sm overflow-hidden group">
		<!-- Placeholder for UI screenshot -->
        {#if imageSrc}
            <img src={imageSrc} alt={title} class="w-full h-full object-cover object-top" />
        {:else}
		    <div class="w-full h-full bg-gray-50 p-4">
                <div class="w-full h-4 bg-gray-200 rounded mb-2"></div>
                <div class="w-3/4 h-4 bg-gray-200 rounded mb-4"></div>
                <div class="space-y-2">
                    <div class="w-full h-2 bg-gray-100 rounded"></div>
                    <div class="w-full h-2 bg-gray-100 rounded"></div>
                    <div class="w-5/6 h-2 bg-gray-100 rounded"></div>
                </div>
            </div>
        {/if}
	</div>
</div>
