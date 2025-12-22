<script lang="ts">
	// Logos
	const logos = [
		{ name: 'Stripe', width: 80 },
		{ name: 'Airbnb', width: 90 },
		{ name: 'Shopify', width: 80 },
		{ name: 'Notion', width: 80 },
		{ name: 'Linear', width: 90 },
		{ name: 'Vercel', width: 80 },
		{ name: 'Figma', width: 80 },
		{ name: 'Slack', width: 80 },
		{ name: 'Discord', width: 90 },
		{ name: 'Webflow', width: 80 }
	];
</script>

<section class="relative pt-32 pb-16 px-6 md:px-12 max-w-7xl mx-auto min-h-screen flex flex-col justify-between">
	<div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
		<div class="z-10">
			<h1 class="text-6xl md:text-7xl lg:text-8xl font-display font-medium text-brand-primary leading-[0.9] tracking-tight mb-8">
				E2E Testing Without the Flakes
			</h1>
			
			<div class="relative w-12 h-12 mb-8">
				<!-- Test icon/illustration -->
				<svg viewBox="0 0 24 24" fill="none" class="w-8 h-8 text-gray-400 absolute top-0 left-0 animate-pulse">
					<path d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z" stroke="currentColor" stroke-width="2" opacity="0.5"/>
				</svg>
			</div>

			<div class="space-y-6 max-w-lg">
				<p class="font-mono text-sm text-brand-primary uppercase tracking-wider leading-relaxed">
					AI-POWERED TEST AUTOMATION<br>
					THAT ELIMINATES FLAKY TESTS<br>
					AND SELENIUM SCRIPT MAINTENANCE
				</p>

				<div class="flex flex-col items-start gap-3">
					<button class="bg-brand-primary text-white px-6 py-3 rounded text-sm font-medium hover:bg-brand-primary-hover transition-colors flex items-center gap-2">
						Start Free Trial 
						<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14"/><path d="m12 5 7 7-7 7"/></svg>
					</button>
					<p class="text-[10px] text-gray-500 font-mono uppercase tracking-wide">
						no credit card required - 14-day free trial
					</p>
				</div>
			</div>
		</div>

		<div class="relative h-[400px] lg:h-[600px] w-full flex items-center justify-center">
			<!-- Testing Dashboard -->
			<div class="absolute inset-0 flex items-center justify-center">
				<img src="/generated/image-a-modern-software-testing-dashboard-on-a-1766369159826-0.webp" alt="Testing Dashboard" class="w-full h-full object-contain rounded-lg shadow-2xl" />
			</div>
		</div>
	</div>

	<div class="mt-20 border-t border-gray-300 pt-8">
		<div class="flex items-center gap-2 text-[10px] font-mono uppercase tracking-wider text-gray-600 mb-6">
			500+ ENGINEERING TEAMS USE PHOSPHOR FOR RELIABLE E2E TESTING. 
			<a href="/" class="text-brand-primary hover:underline flex items-center gap-1">
				SEE WHY TEAMS <span class="text-xs">♥</span> PHOSPHOR ->
			</a>
		</div>
		
		<div class="grid grid-cols-2 md:grid-cols-5 gap-8 opacity-60 grayscale">
			{#each logos as logo}
				<div class="h-8 flex items-center justify-center border border-gray-300/50 rounded bg-gray-100/50">
					<span class="text-xs font-bold text-gray-500">{logo.name}</span>
				</div>
			{/each}
		</div>
	</div>
</section>
