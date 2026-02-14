<script lang="ts">
	const modules = [
		{
			icon: '⚡',
			name: 'Operator System',
			audience: 'For Founders & Executives',
			price: '+$1,000–$1,500/mo',
			features: [
				'Deal tracking & pipeline visibility',
				'Client follow-up automation',
				'Proposal & document drafting',
				'Revenue summary briefings',
				'Strategic planning support'
			]
		},
		{
			icon: '🏠',
			name: 'Household CEO',
			audience: 'For Affluent Families',
			price: '+$500–$1,000/mo',
			features: [
				'Family calendar optimization',
				'Kids activity & schedule management',
				'Travel coordination & planning',
				'Vendor & home services tracking',
				'Household budget intelligence'
			]
		},
		{
			icon: '📈',
			name: 'Wealth Builder',
			audience: 'For Investors & High Earners',
			price: '+$750–$1,500/mo',
			features: [
				'Investment briefings & alerts',
				'Expense oversight & categorization',
				'Tax prep summaries',
				'Capital event reminders',
				'Financial snapshot reports'
			]
		},
		{
			icon: '🎯',
			name: 'Creator Engine',
			audience: 'For Consultants & Creators',
			price: '+$750–$1,250/mo',
			features: [
				'Content ideation & research',
				'Voice calibration & brand consistency',
				'Repurposing workflows',
				'Publishing preparation',
				'Audience analytics summaries'
			]
		}
	];

	const faqs = [
		{
			q: 'How is this different from ChatGPT or other AI tools?',
			a: 'ChatGPT is a chat window. OpenClaw is infrastructure. Your AI Chief of Staff runs 24/7 on your hardware, connected to your email, calendar, CRM, and tools. It acts proactively — triaging your inbox, drafting responses, generating briefings — without you opening a browser.'
		},
		{
			q: 'Do I need to be technical?',
			a: 'Not at all. We handle everything: deployment, security hardening, integrations, and ongoing maintenance. You interact with your AI through email, Slack, or text — however you prefer.'
		},
		{
			q: 'Who owns the AI and the data?',
			a: 'You do. 100%. Your system runs on your infrastructure, uses your API keys, and your data never touches our servers. If you ever want to part ways, you keep everything.'
		},
		{
			q: 'What AI models do you use?',
			a: 'We configure your system with the best models for each task — Claude, GPT, Gemini, or others. You pay the AI providers directly at their standard rates. No markup from us.'
		},
		{
			q: 'How long does setup take?',
			a: 'Most deployments are live within 5–7 business days. That includes a discovery call, configuration, integration setup, testing, and a 14-day hypercare period where we fine-tune everything.'
		},
		{
			q: 'Can I add modules later?',
			a: 'Absolutely. Most clients start with the base AI Chief of Staff and add modules as they see the value. There is no long-term contract — scale up or down as needed.'
		}
	];

	let openFaq = $state<number | null>(null);

	function toggleFaq(i: number) {
		openFaq = openFaq === i ? null : i;
	}
</script>

<!-- Nav -->
<nav class="fixed top-0 w-full z-50 bg-[#1a1a2e]/95 backdrop-blur-sm border-b border-white/5">
	<div class="max-w-6xl mx-auto px-6 py-4 flex items-center justify-between">
		<div class="text-xl font-bold text-white tracking-tight">
			Open<span class="text-[#6c63ff]">Claw</span>
		</div>
		<a
			href="#book"
			class="bg-[#6c63ff] hover:bg-[#8b83ff] text-white px-5 py-2.5 rounded-lg font-semibold text-sm transition-colors"
		>
			Book a Discovery Call
		</a>
	</div>
</nav>

<!-- Hero -->
<section class="min-h-screen flex items-center bg-gradient-to-b from-[#1a1a2e] via-[#1a1a2e] to-[#16213e] pt-20">
	<div class="max-w-6xl mx-auto px-6 py-20">
		<div class="max-w-3xl">
			<div class="inline-block bg-[#6c63ff]/10 border border-[#6c63ff]/20 rounded-full px-4 py-1.5 text-[#6c63ff] text-sm font-medium mb-8">
				Private AI Infrastructure
			</div>
			<h1 class="text-5xl md:text-6xl lg:text-7xl font-extrabold text-white leading-[1.1] mb-6">
				Your AI Chief of Staff.
				<span class="text-[#6c63ff] block mt-2">Configured. Secured. Maintained.</span>
			</h1>
			<p class="text-xl text-gray-400 mb-10 max-w-2xl leading-relaxed">
				We deploy private AI systems for founders, executives, and affluent households.
				Your inbox triaged. Your calendar optimized. Your follow-ups tracked.
				Running 24/7 on your hardware. Owned by you.
			</p>
			<div class="flex flex-col sm:flex-row gap-4">
				<a
					href="#book"
					class="bg-[#6c63ff] hover:bg-[#8b83ff] text-white px-8 py-4 rounded-lg font-semibold text-lg transition-colors text-center"
				>
					Book a Discovery Call
				</a>
				<a
					href="#how"
					class="border border-white/20 hover:border-white/40 text-white px-8 py-4 rounded-lg font-semibold text-lg transition-colors text-center"
				>
					See How It Works
				</a>
			</div>
			<div class="mt-12 flex flex-wrap items-center gap-6 text-sm text-gray-500">
				<span class="flex items-center gap-2">
					<span class="w-2 h-2 bg-green-500 rounded-full"></span>
					Client-owned infrastructure
				</span>
				<span class="flex items-center gap-2">
					<span class="w-2 h-2 bg-green-500 rounded-full"></span>
					No token markup
				</span>
				<span class="flex items-center gap-2">
					<span class="w-2 h-2 bg-green-500 rounded-full"></span>
					14-day hypercare included
				</span>
			</div>
		</div>
	</div>
</section>

<!-- Problem -->
<section class="bg-[#16213e] py-24">
	<div class="max-w-6xl mx-auto px-6">
		<div class="text-center mb-16">
			<h2 class="text-3xl md:text-4xl font-bold text-white mb-4">Sound Familiar?</h2>
			<p class="text-gray-400 text-lg max-w-2xl mx-auto">
				You're successful. But your day is consumed by operational noise.
			</p>
		</div>
		<div class="grid md:grid-cols-3 gap-8">
			<div class="bg-[#1a1a2e]/50 border border-white/5 rounded-2xl p-8">
				<div class="text-4xl mb-4">📧</div>
				<h3 class="text-xl font-semibold text-white mb-3">Drowning in Email</h3>
				<p class="text-gray-400">
					47 unread before breakfast. Important messages buried under newsletters and noise.
					You spend 90+ minutes daily just triaging.
				</p>
			</div>
			<div class="bg-[#1a1a2e]/50 border border-white/5 rounded-2xl p-8">
				<div class="text-4xl mb-4">📅</div>
				<h3 class="text-xl font-semibold text-white mb-3">Calendar Chaos</h3>
				<p class="text-gray-400">
					Double-bookings. No buffer time. Scheduling conflicts you discover 5 minutes before the call.
					Your calendar runs you, not the other way around.
				</p>
			</div>
			<div class="bg-[#1a1a2e]/50 border border-white/5 rounded-2xl p-8">
				<div class="text-4xl mb-4">🧠</div>
				<h3 class="text-xl font-semibold text-white mb-3">Everything Slips Through</h3>
				<p class="text-gray-400">
					Follow-ups you forgot. Promises you made in meetings last month.
					The mental load of keeping track of everything is the real bottleneck.
				</p>
			</div>
		</div>
	</div>
</section>

<!-- Solution / What You Get -->
<section class="bg-[#1a1a2e] py-24">
	<div class="max-w-6xl mx-auto px-6">
		<div class="text-center mb-16">
			<h2 class="text-3xl md:text-4xl font-bold text-white mb-4">What You Wake Up To Instead</h2>
			<p class="text-gray-400 text-lg max-w-2xl mx-auto">
				Your AI Chief of Staff handles the operational noise so you can focus on what matters.
			</p>
		</div>
		<div class="bg-[#16213e] border border-white/10 rounded-2xl p-8 md:p-12 max-w-4xl mx-auto">
			<div class="space-y-6">
				{#each [
					{ n: '1', title: 'Inbox Triaged & Prioritized', desc: '3 emails flagged as urgent with draft responses ready. 12 emails categorized as FYI-only and archived. Zero noise.' },
					{ n: '2', title: 'Calendar Optimized', desc: 'Conflicts resolved. Travel time added. Buffer periods protected. Your day structured for peak performance.' },
					{ n: '3', title: 'Daily Briefing at 6am', desc: "Today's priorities, pending follow-ups with context from previous conversations, and key metrics — all in one place." },
					{ n: '4', title: 'Follow-ups Tracked Automatically', desc: 'Every commitment logged. Every promise remembered. Nothing falls through the cracks because your AI never forgets.' },
					{ n: '5', title: 'Research On Demand', desc: 'Ask a question in plain English. Get a researched answer with sources. Competitive analysis, market data, or prep for your next meeting.' }
				] as item}
					<div class="flex items-start gap-4">
						<div class="w-10 h-10 bg-[#6c63ff]/20 rounded-lg flex items-center justify-center shrink-0 text-[#6c63ff] font-bold">{item.n}</div>
						<div>
							<h3 class="text-lg font-semibold text-white">{item.title}</h3>
							<p class="text-gray-400">{item.desc}</p>
						</div>
					</div>
				{/each}
			</div>
			<div class="mt-10 pt-8 border-t border-white/10 text-center">
				<p class="text-gray-400 text-lg">
					<span class="text-white font-semibold">10 minutes reviewing</span> instead of <span class="text-white font-semibold">90 minutes drowning.</span>
				</p>
			</div>
		</div>
	</div>
</section>

<!-- How It Works -->
<section id="how" class="bg-[#16213e] py-24">
	<div class="max-w-6xl mx-auto px-6">
		<div class="text-center mb-16">
			<h2 class="text-3xl md:text-4xl font-bold text-white mb-4">How It Works</h2>
			<p class="text-gray-400 text-lg max-w-2xl mx-auto">
				From first call to live system in under two weeks.
			</p>
		</div>
		<div class="grid md:grid-cols-3 gap-8">
			{#each [
				{ n: '1', title: 'Discover', desc: "30-minute call. We learn your workflow, tools, and priorities. You tell us what eats your time. We design the system." },
				{ n: '2', title: 'Deploy', desc: 'We configure your private AI infrastructure. Integrations connected. Security hardened. Workflows tested with your real data.' },
				{ n: '3', title: 'Optimize', desc: "14-day hypercare. We fine-tune based on how you actually use it. Then ongoing managed care to keep everything running perfectly." }
			] as step}
				<div class="text-center">
					<div class="w-16 h-16 bg-[#6c63ff]/20 rounded-2xl flex items-center justify-center mx-auto mb-6">
						<span class="text-[#6c63ff] text-2xl font-bold">{step.n}</span>
					</div>
					<h3 class="text-xl font-semibold text-white mb-3">{step.title}</h3>
					<p class="text-gray-400">{step.desc}</p>
				</div>
			{/each}
		</div>
	</div>
</section>

<!-- Modules -->
<section class="bg-[#1a1a2e] py-24">
	<div class="max-w-6xl mx-auto px-6">
		<div class="text-center mb-16">
			<h2 class="text-3xl md:text-4xl font-bold text-white mb-4">Expansion Modules</h2>
			<p class="text-gray-400 text-lg max-w-2xl mx-auto">
				Start with the AI Chief of Staff base. Add modules based on your identity and needs.
			</p>
		</div>
		<div class="grid md:grid-cols-2 gap-8">
			{#each modules as mod}
				<div class="bg-[#16213e] border border-white/10 rounded-2xl p-8 hover:border-[#6c63ff]/30 transition-colors">
					<div class="flex items-center gap-3 mb-4">
						<span class="text-3xl">{mod.icon}</span>
						<div>
							<h3 class="text-xl font-semibold text-white">{mod.name}</h3>
							<p class="text-[#6c63ff] text-sm font-medium">{mod.audience}</p>
						</div>
					</div>
					<ul class="space-y-2 mb-6">
						{#each mod.features as feat}
							<li class="flex items-center gap-2 text-gray-400">
								<span class="text-[#6c63ff] text-sm">&#10003;</span>
								{feat}
							</li>
						{/each}
					</ul>
					<div class="text-[#d4af37] font-semibold text-sm">{mod.price}</div>
				</div>
			{/each}
		</div>
	</div>
</section>

<!-- Pricing -->
<section class="bg-[#16213e] py-24">
	<div class="max-w-6xl mx-auto px-6">
		<div class="text-center mb-16">
			<h2 class="text-3xl md:text-4xl font-bold text-white mb-4">Investment</h2>
			<p class="text-gray-400 text-lg max-w-2xl mx-auto">
				Less than a part-time executive assistant. Available 24/7.
			</p>
		</div>
		<div class="grid md:grid-cols-3 gap-8 max-w-5xl mx-auto">
			<!-- Good -->
			<div class="bg-[#1a1a2e] border border-white/10 rounded-2xl p-8">
				<h3 class="text-lg font-semibold text-white mb-1">AI Chief of Staff</h3>
				<p class="text-gray-500 text-sm mb-6">The foundation</p>
				<div class="mb-2">
					<span class="text-4xl font-bold text-white">$2,500</span>
					<span class="text-gray-400"> setup</span>
				</div>
				<div class="mb-8">
					<span class="text-2xl font-bold text-white">$1,500</span>
					<span class="text-gray-400">/month</span>
				</div>
				<ul class="space-y-3 mb-8">
					{#each ['Inbox prioritization & drafting', 'Calendar intelligence', 'Daily & weekly briefings', 'Follow-up tracking', 'Research assistance', 'Security hardening', '14-day hypercare'] as f}
						<li class="flex items-start gap-2 text-gray-400 text-sm">
							<span class="text-[#6c63ff] mt-0.5">&#10003;</span>{f}
						</li>
					{/each}
				</ul>
				<a href="#book" class="block text-center border border-white/20 hover:border-white/40 text-white py-3 rounded-lg font-semibold transition-colors">
					Get Started
				</a>
			</div>

			<!-- Better -->
			<div class="bg-[#1a1a2e] border-2 border-[#6c63ff] rounded-2xl p-8 relative">
				<div class="absolute -top-3 left-1/2 -translate-x-1/2 bg-[#6c63ff] text-white text-xs font-bold px-4 py-1 rounded-full">
					MOST POPULAR
				</div>
				<h3 class="text-lg font-semibold text-white mb-1">Chief of Staff + Module</h3>
				<p class="text-gray-500 text-sm mb-6">Best value</p>
				<div class="mb-2">
					<span class="text-4xl font-bold text-white">$2,500</span>
					<span class="text-gray-400"> setup</span>
				</div>
				<div class="mb-8">
					<span class="text-2xl font-bold text-white">$2,500–$3,000</span>
					<span class="text-gray-400">/mo</span>
				</div>
				<ul class="space-y-3 mb-8">
					{#each ['Everything in base', '1 expansion module of your choice', 'Custom workflow configuration', 'Monthly optimization calls', 'Priority support channel'] as f}
						<li class="flex items-start gap-2 text-gray-400 text-sm">
							<span class="text-[#6c63ff] mt-0.5">&#10003;</span>
							{#if f.includes('expansion')}<strong class="text-white">{f}</strong>{:else}{f}{/if}
						</li>
					{/each}
				</ul>
				<a href="#book" class="block text-center bg-[#6c63ff] hover:bg-[#8b83ff] text-white py-3 rounded-lg font-semibold transition-colors">
					Book a Call
				</a>
			</div>

			<!-- Best -->
			<div class="bg-[#1a1a2e] border border-[#d4af37]/30 rounded-2xl p-8">
				<h3 class="text-lg font-semibold text-white mb-1">Full Suite</h3>
				<p class="text-gray-500 text-sm mb-6">Maximum leverage</p>
				<div class="mb-2">
					<span class="text-4xl font-bold text-white">$5,000</span>
					<span class="text-gray-400"> setup</span>
				</div>
				<div class="mb-8">
					<span class="text-2xl font-bold text-white">$4,000–$5,000</span>
					<span class="text-gray-400">/mo</span>
				</div>
				<ul class="space-y-3 mb-8">
					{#each ['Everything in base', '2–3 expansion modules', 'Advanced workflow automation', 'Dedicated support channel', 'Quarterly security reviews', 'White-glove onboarding'] as f}
						<li class="flex items-start gap-2 text-gray-400 text-sm">
							<span class="text-[#6c63ff] mt-0.5">&#10003;</span>
							{#if f.includes('expansion')}<strong class="text-white">{f}</strong>{:else}{f}{/if}
						</li>
					{/each}
				</ul>
				<a href="#book" class="block text-center border border-[#d4af37]/40 hover:border-[#d4af37] text-[#d4af37] py-3 rounded-lg font-semibold transition-colors">
					Contact Us
				</a>
			</div>
		</div>
		<p class="text-center text-gray-500 text-sm mt-8">
			You pay AI providers (Anthropic, OpenAI) directly. We never mark up token costs.
		</p>
	</div>
</section>

<!-- Trust -->
<section class="bg-[#1a1a2e] py-24">
	<div class="max-w-6xl mx-auto px-6">
		<div class="text-center mb-16">
			<h2 class="text-3xl md:text-4xl font-bold text-white mb-4">Why OpenClaw</h2>
		</div>
		<div class="grid md:grid-cols-2 lg:grid-cols-4 gap-6">
			{#each [
				{ icon: '🔒', title: 'You Own Everything', desc: 'Your hardware. Your API keys. Your data. No vendor lock-in.' },
				{ icon: '💰', title: 'No Token Markup', desc: 'Pay AI providers directly at their standard rates. We charge for architecture, not compute.' },
				{ icon: '🛡️', title: 'Security First', desc: 'Hardened deployment. Encrypted credentials. Audit trails. Your data never touches our servers.' },
				{ icon: '🧩', title: 'Modular by Design', desc: "Start with what you need. Add modules as you grow. No paying for features you don't use." }
			] as item}
				<div class="text-center p-6">
					<div class="text-3xl mb-4">{item.icon}</div>
					<h3 class="text-white font-semibold mb-2">{item.title}</h3>
					<p class="text-gray-400 text-sm">{item.desc}</p>
				</div>
			{/each}
		</div>
	</div>
</section>

<!-- FAQ -->
<section class="bg-[#16213e] py-24">
	<div class="max-w-3xl mx-auto px-6">
		<div class="text-center mb-16">
			<h2 class="text-3xl md:text-4xl font-bold text-white mb-4">Questions</h2>
		</div>
		<div class="space-y-4">
			{#each faqs as faq, i}
				<button
					class="w-full text-left bg-[#1a1a2e] border border-white/10 rounded-xl p-6 hover:border-white/20 transition-colors"
					onclick={() => toggleFaq(i)}
				>
					<div class="flex items-center justify-between">
						<h3 class="text-white font-semibold pr-4">{faq.q}</h3>
						<span class="text-[#6c63ff] text-xl shrink-0">{openFaq === i ? '−' : '+'}</span>
					</div>
					{#if openFaq === i}
						<p class="text-gray-400 mt-4 leading-relaxed">{faq.a}</p>
					{/if}
				</button>
			{/each}
		</div>
	</div>
</section>

<!-- Final CTA -->
<section id="book" class="bg-gradient-to-b from-[#16213e] to-[#1a1a2e] py-24">
	<div class="max-w-3xl mx-auto px-6 text-center">
		<h2 class="text-3xl md:text-4xl font-bold text-white mb-6">
			Ready to Get Your Time Back?
		</h2>
		<p class="text-gray-400 text-lg mb-10 max-w-xl mx-auto">
			Book a 30-minute discovery call. We'll learn your workflow and show you exactly how
			your AI Chief of Staff would work. No commitment. No pitch deck. Just a conversation.
		</p>
		<a
			href="https://calendly.com"
			target="_blank"
			rel="noopener noreferrer"
			class="inline-block bg-[#6c63ff] hover:bg-[#8b83ff] text-white px-10 py-4 rounded-lg font-semibold text-lg transition-colors"
		>
			Book Your Discovery Call
		</a>
		<p class="text-gray-600 text-sm mt-6">Currently accepting a limited number of new clients.</p>
	</div>
</section>

<!-- Footer -->
<footer class="bg-[#1a1a2e] border-t border-white/5 py-12">
	<div class="max-w-6xl mx-auto px-6">
		<div class="flex flex-col md:flex-row items-center justify-between gap-4">
			<div class="text-white font-bold text-lg">
				Open<span class="text-[#6c63ff]">Claw</span>
			</div>
			<p class="text-gray-600 text-sm">
				We sell architecture and leverage, not compute.
			</p>
			<p class="text-gray-600 text-sm">
				&copy; {new Date().getFullYear()} OpenClaw. All rights reserved.
			</p>
		</div>
	</div>
</footer>
