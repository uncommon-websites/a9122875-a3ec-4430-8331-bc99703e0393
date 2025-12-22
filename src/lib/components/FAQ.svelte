<script lang="ts">
	import { slide } from 'svelte/transition';

	const faqs = [
		{
			question: "How does Phosphor pricing work?",
			answer: "Phosphor charges based on the number of test runs per month. We offer flexible plans for teams of all sizes, from startups to enterprises."
		},
		{
			question: "Can Phosphor be self-hosted?",
			answer: "Yes, Phosphor can be deployed in your own VPC or on-premise environment. Contact us for enterprise pricing and deployment options."
		},
		{
			question: "Are there free trials or discounts available for Phosphor?",
			answer: "Yes, we offer a 14-day free trial with no credit card required. We also offer discounts for startups and open source projects."
		},
		{
			question: "What frameworks and technologies does Phosphor support?",
			answer: "Phosphor supports all major web frameworks including React, Vue, Angular, Svelte, and more. We work with any application that runs in a browser."
		},
		{
			question: "How does Phosphor handle test maintenance?",
			answer: "Phosphor uses AI to automatically adapt tests when your UI changes. Our self-healing technology updates selectors and flows so you don't have to."
		},
		{
			question: "Can I integrate Phosphor with my CI/CD pipeline?",
			answer: "Yes, Phosphor integrates seamlessly with GitHub Actions, GitLab CI, CircleCI, Jenkins, and all major CI/CD platforms."
		},
		{
			question: "What is AI-powered test automation?",
			answer: "AI-powered test automation uses machine learning to generate, maintain, and heal E2E tests automatically. It understands your application and creates tests based on user flows described in plain English."
		}
	];

	let openIndex: number | null = null;

	function toggle(index: number) {
		openIndex = openIndex === index ? null : index;
	}
</script>

<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto border-t border-gray-200">
	<div class="grid grid-cols-1 lg:grid-cols-3 gap-12">
		<div>
			<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
				[ FAQ ]
			</span>
			<h2 class="font-display text-4xl md:text-5xl font-medium tracking-tight text-gray-900 mb-6">
				Frequently Asked Questions
			</h2>
			<p class="font-mono text-sm text-gray-600 mb-8">
				Your question not answered here?
			</p>
			<button class="bg-brand-primary text-white px-5 py-2.5 rounded text-sm font-medium hover:bg-brand-primary-hover transition-colors flex items-center gap-2 font-mono uppercase tracking-wide text-xs">
				<svg xmlns="http://www.w3.org/2000/svg" width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"/></svg>
				Contact Us
			</button>
		</div>

		<div class="lg:col-span-2 space-y-4">
			{#each faqs as faq, i}
				<div class="border-b border-gray-200 pb-4">
					<button class="w-full flex items-center justify-between text-left py-2 group" on:click={() => toggle(i)}>
						<span class="font-mono text-sm font-medium text-gray-800 group-hover:text-brand-primary transition-colors pr-8">{faq.question}</span>
						<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="text-gray-400 transition-transform duration-300 {openIndex === i ? 'rotate-180' : ''}"><path d="m6 9 6 6 6-6"/></svg>
					</button>
					{#if openIndex === i}
						<div transition:slide={{ duration: 300 }} class="overflow-hidden">
							<p class="pt-2 pb-4 text-sm text-gray-600 leading-relaxed max-w-2xl font-mono">
								{faq.answer}
							</p>
						</div>
					{/if}
				</div>
			{/each}
		</div>
	</div>
</section>
