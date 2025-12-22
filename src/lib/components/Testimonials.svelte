<script lang="ts">
	const testimonials = [
		{
			quote: "Phosphor eliminated our flaky test problem overnight. We went from spending 15 hours a week maintaining Selenium tests to basically zero maintenance. It's incredible.",
			author: "Sarah",
			role: "QA Manager • Stripe",
			image: "https://i.pravatar.cc/150?u=sarah",
            icon: "https://placehold.co/20x20/635BFF/fff?text=S"
		},
		{
			quote: "The AI test generation is mind-blowing. I describe a user flow in plain English and Phosphor creates comprehensive E2E tests. Our test coverage went from 40% to 85% in two months.",
			author: "Marcus",
			role: "Frontend Lead • Airbnb",
			image: "https://i.pravatar.cc/150?u=marcus",
            icon: "https://placehold.co/20x20/FF5A5F/fff?text=A"
		},
		{
			quote: "Finally, a testing platform that doesn't require a dedicated QA team to maintain. Phosphor just works. Our engineers can focus on building features instead of fixing tests.",
			author: "Priya",
			role: "Engineering Manager • Notion",
			image: "https://i.pravatar.cc/150?u=priya",
            icon: "https://placehold.co/20x20/000/fff?text=N"
		},
		{
			quote: "We switched from manual E2E testing to Phosphor and cut our release cycle from 2 weeks to 3 days. The self-healing tests are a game-changer.",
			author: "David",
			role: "CTO • Linear",
			image: "https://i.pravatar.cc/150?u=david",
            icon: "https://placehold.co/20x20/5E6AD2/fff?text=L"
		},
		{
			quote: "Setup took 10 minutes. Within a day we had 50+ AI-generated tests running on every commit. Best developer tool investment we've made this year.",
			author: "Emma",
			role: "Product Manager • Vercel",
			image: "https://i.pravatar.cc/150?u=emma",
            icon: "https://placehold.co/20x20/000/fff?text=V"
		},
		{
			quote: "Phosphor's managed infrastructure means we don't worry about browser versions, parallelization, or scaling. It just runs our tests fast and reliably.",
			author: "Alex",
			role: "DevOps Lead • Figma",
			image: "https://i.pravatar.cc/150?u=alex",
            icon: "https://placehold.co/20x20/000/fff?text=F"
		},
        {
			quote: "The self-healing feature is magic. We refactored our entire component library and 90% of our tests adapted automatically. Saved us weeks of work.",
			author: "Jordan",
			role: "QA Engineer • Slack",
			image: "https://i.pravatar.cc/150?u=jordan",
            icon: "https://placehold.co/20x20/4A154B/fff?text=S"
		},
        {
			quote: "As a frontend engineer, I was skeptical about AI testing. Phosphor proved me wrong. The tests it generates are actually better than what I was writing manually.",
			author: "Taylor",
			role: "Senior Engineer • Discord",
			image: "https://i.pravatar.cc/150?u=taylor",
            icon: "https://placehold.co/20x20/5865F2/fff?text=D"
		}
	];
</script>

<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto">
	<div class="text-center mb-16">
		<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
			[ TESTIMONIALS ]
		</span>
		<h2 class="font-display text-4xl md:text-5xl font-medium tracking-tight text-gray-900 mb-4">
			From Teams That Use Phosphor
		</h2>
		<p class="font-mono text-sm text-gray-600">
			See what engineering teams are saying about their experience with Phosphor
		</p>
	</div>

	<div class="columns-1 md:columns-2 lg:columns-3 gap-6 space-y-6">
		{#each testimonials as t}
			<div class="bg-white p-6 rounded-lg border border-gray-200 shadow-sm break-inside-avoid hover:shadow-md transition-shadow">
				<p class="font-mono text-xs leading-relaxed text-gray-700 mb-6">
					"{t.quote}"
				</p>
				<div class="flex items-center justify-between border-t border-gray-100 pt-4">
					<div class="flex items-center gap-3">
						<img src={t.image} alt={t.author} class="w-8 h-8 rounded-full bg-gray-200" />
						<div>
							<div class="text-xs font-bold text-gray-900">{t.author}</div>
							<div class="text-[10px] text-gray-500 font-mono">{t.role}</div>
						</div>
					</div>
                    <img src={t.icon} alt="Company Logo" class="w-5 h-5 rounded-sm opacity-70 grayscale" />
				</div>
			</div>
		{/each}
	</div>
</section>
