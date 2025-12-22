<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto bg-[#EAEAE8]">
	<div class="text-center mb-16">
		<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
			[ DATA-DRIVEN RESULTS ]
		</span>
		<h2 class="font-display text-4xl md:text-5xl lg:text-6xl font-medium tracking-tight text-gray-900 mb-8">
			Ship with confidence using Phosphor.
		</h2>
		<button class="bg-black text-white px-5 py-2.5 rounded text-sm font-medium hover:bg-gray-800 transition-colors inline-flex items-center gap-2 font-mono uppercase tracking-wide text-xs">
			<svg xmlns="http://www.w3.org/2000/svg" width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M3 3v18h18"/><path d="m19 9-5 5-4-4-3 3"/></svg>
			View performance data
		</button>
	</div>

	<div class="grid grid-cols-1 md:grid-cols-2 gap-8">
		<!-- Chart 1 -->
		<div class="bg-[#F3F3F1] p-6 rounded-lg border border-gray-200">
			<h3 class="font-mono text-xs text-gray-500 uppercase mb-8">Test Maintenance Time Comparison</h3>
			<div class="h-64 relative flex items-end justify-center gap-16 pb-8">
				<!-- Bar 1 -->
				<div class="flex flex-col items-center gap-2 group">
					<span class="text-xs text-gray-500 font-mono mb-1 group-hover:text-gray-900">Manual Tests</span>
					<div class="w-16 bg-gray-300 rounded-t h-48 relative group-hover:bg-gray-400 transition-colors"></div>
					<span class="font-display text-xl font-medium">15 hrs/wk</span>
				</div>
				
				<!-- Bar 2 -->
				<div class="flex flex-col items-center gap-2 group">
					<span class="text-xs text-brand-primary font-mono mb-1 font-bold">WITH PHOSPHOR</span>
					<div class="w-16 bg-brand-primary rounded-t h-12 relative group-hover:bg-brand-primary-hover transition-colors">
                        <div class="absolute -top-8 left-1/2 -translate-x-1/2">
                            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="currentColor" class="text-brand-primary"><path d="M12 2L15 8L21 9L17 14L18 20L12 17L6 20L7 14L3 9L9 8L12 2Z"/></svg>
                        </div>
                    </div>
					<span class="font-display text-xl font-medium text-brand-primary">2 hrs/wk</span>
				</div>
			</div>
		</div>

		<!-- Chart 2 -->
		<div class="bg-[#F3F3F1] p-6 rounded-lg border border-gray-200">
			<h3 class="font-mono text-xs text-gray-500 uppercase mb-8">Test Coverage Over Time</h3>
			<div class="h-64 relative w-full">
                <!-- Simple SVG Line Chart -->
                <svg viewBox="0 0 300 200" class="w-full h-full overflow-visible">
                    <!-- Axes -->
                    <line x1="0" y1="200" x2="300" y2="200" stroke="#ddd" stroke-width="1" />
                    <line x1="0" y1="0" x2="0" y2="200" stroke="#ddd" stroke-width="1" />
                    
                    <!-- Line 1: Manual Tests (Declining) -->
                    <path d="M0,100 Q100,120 150,140 T300,180" fill="none" stroke="#9CA3AF" stroke-width="2" stroke-dasharray="4 4" />
                    <text x="180" y="170" font-family="monospace" font-size="10" fill="#6B7280">Manual Tests</text>
                    
                    <!-- Line 2: With Phosphor (Increasing) -->
                    <path d="M0,180 Q100,120 150,60 T300,20" fill="none" stroke="oklch(0.637 0.237 25.331)" stroke-width="2" />
                    <text x="180" y="50" font-family="monospace" font-size="10" fill="oklch(0.637 0.237 25.331)" font-weight="bold">WITH PHOSPHOR</text>
                </svg>
			</div>
            <div class="flex justify-between mt-4 text-[10px] text-gray-400 font-mono uppercase">
                <span>Time -></span>
                <span>Coverage % -></span>
            </div>
		</div>
	</div>
</section>
