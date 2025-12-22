<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto relative overflow-hidden">
	<div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center relative z-10">
		<div>
			<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
				[ INTELLIGENT TESTING ]
			</span>
			<h2 class="font-display text-4xl md:text-5xl lg:text-6xl font-medium tracking-tight text-gray-900 mb-6 leading-[0.95]">
				Self-healing<br>tests.
			</h2>
			<p class="font-mono text-sm text-gray-600 max-w-md mb-8 leading-relaxed">
				Phosphor's AI automatically adapts tests when your UI changes. Tests update themselves when you refactor components, change IDs, or restructure your DOM.
			</p>
			
			<button class="bg-black text-white px-5 py-2.5 rounded text-sm font-medium hover:bg-gray-800 transition-colors flex items-center gap-2 font-mono uppercase tracking-wide text-xs w-fit">
				<span class="text-accent-yellow">✦</span> See how it works
			</button>
		</div>

		<div class="relative h-[400px] w-full flex items-center justify-center">
			<!-- Background Text Pattern -->
            <div class="absolute inset-0 flex flex-col items-center justify-center opacity-5 select-none pointer-events-none overflow-hidden leading-none">
                {#each Array(10) as _, i}
                    <div class="text-6xl md:text-8xl font-black text-gray-900 whitespace-nowrap">
                        TESTING TESTING TESTING
                    </div>
                {/each}
            </div>

            <!-- Floating Cards -->
            <div class="relative z-10 flex flex-col gap-4 w-full max-w-md">
                <div class="bg-white p-4 rounded shadow-lg border border-gray-200 transform -rotate-2 translate-x-4">
                    <div class="flex items-center gap-2 mb-2">
                        <span class="bg-brand-primary text-white text-[10px] font-bold px-1.5 py-0.5 rounded uppercase">Auto-Fixed</span>
                        <span class="text-xs text-gray-500">Just now</span>
                    </div>
                    <p class="text-sm font-mono text-gray-800">Button selector updated after refactor</p>
                </div>

                <div class="bg-white p-4 rounded shadow-lg border border-gray-200 transform rotate-1 translate-x-8">
                    <div class="flex items-center gap-2 mb-2">
                        <span class="bg-brand-primary text-white text-[10px] font-bold px-1.5 py-0.5 rounded uppercase">Auto-Fixed</span>
                        <span class="text-xs text-gray-500">2h ago</span>
                    </div>
                    <p class="text-sm font-mono text-gray-800">Form validation flow adapted to new UI</p>
                </div>

                 <div class="bg-white p-4 rounded shadow-lg border border-gray-200 transform -rotate-1">
                    <div class="flex items-center gap-2 mb-2">
                        <span class="bg-brand-primary text-white text-[10px] font-bold px-1.5 py-0.5 rounded uppercase">Auto-Fixed</span>
                        <span class="text-xs text-gray-500">1d ago</span>
                    </div>
                    <p class="text-sm font-mono text-gray-800">Navigation test updated for new menu</p>
                </div>
            </div>
		</div>
	</div>
</section>
