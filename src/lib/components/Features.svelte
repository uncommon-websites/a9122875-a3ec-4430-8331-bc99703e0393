<script lang="ts">
	import FeatureCard from './FeatureCard.svelte';
</script>

<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto relative" id="features">
    <!-- Background Grid Pattern -->
    <div class="absolute inset-0 z-0 opacity-30 pointer-events-none" 
        style="background-image: linear-gradient(#ccc 1px, transparent 1px), linear-gradient(90deg, #ccc 1px, transparent 1px); background-size: 40px 40px; mask-image: linear-gradient(to bottom, transparent, black 10%, black 90%, transparent);">
    </div>

	<div class="flex flex-col md:flex-row justify-between items-start md:items-end mb-16 gap-6 relative z-10">
		<div>
			<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
				[ TEST WITH CONFIDENCE ]
			</span>
			<h2 class="font-display text-4xl md:text-5xl lg:text-6xl font-medium tracking-tight text-gray-900 mb-4">
				Testing that just works.
			</h2>
			<p class="font-mono text-sm text-gray-600 max-w-lg">
				Phosphor uses AI to generate and maintain reliable E2E tests, with fully managed infrastructure.
			</p>
		</div>
		
		<button class="bg-black text-white px-5 py-2.5 rounded text-sm font-medium hover:bg-gray-800 transition-colors flex items-center gap-2 font-mono uppercase tracking-wide text-xs">
			See Phosphor in action ->
		</button>
	</div>

	<div class="grid grid-cols-1 md:grid-cols-2 gap-6">
		<FeatureCard 
			subtitle="[ AI-POWERED TESTS ]"
			title="Tests that write<br>themselves"
			description="AI generates comprehensive E2E tests by understanding your application flow and user journeys."
			tagColor="bg-brand-primary"
			tagIcon="arrow"
            imageSrc="/generated/image-close-up-of-hands-typing-code-on-a-lapto-1766369162592-1.webp"
		/>
		
		<FeatureCard 
			subtitle="[ ZERO MAINTENANCE ]"
			title="No more flaky<br>Selenium scripts"
			description="Phosphor automatically adapts tests when your UI changes. Say goodbye to brittle selectors."
			tagColor="bg-accent-orange"
			tagIcon="plus"
            imageSrc="/generated/image-software-engineer-looking-relieved-and-h-1766369164950-2.webp"
		/>
		
		<FeatureCard 
			subtitle="[ MANAGED INFRASTRUCTURE ]"
			title="Fully managed test<br>infrastructure"
			description="We handle browsers, parallelization, and scaling. You just see the results."
			tagColor="bg-accent-pink"
			tagIcon="arrow"
            imageSrc="/generated/image-modern-server-room-with-organized-cables-1766369167260-3.webp"
		/>
		
		<FeatureCard 
			subtitle="[ CI/CD INTEGRATION ]"
			title="Seamless integration<br>with your workflow"
			description="Works with GitHub Actions, GitLab CI, CircleCI, Jenkins, and all major CI/CD platforms."
			tagColor="bg-accent-yellow"
			tagIcon="plus"
            imageSrc="/generated/image-developer-working-on-multiple-monitors-s-1766369209648-4.webp"
		/>
	</div>
</section>
