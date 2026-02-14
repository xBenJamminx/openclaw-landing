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
			audience: 'For Busy Families',
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
			name: 'Finance Module',
			audience: 'For Investors & Business Owners',
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
<nav class="fixed top-0 w-full z-50 frosted border-b border-gray-200/60">
	<div class="max-w-7xl mx-auto px-6 lg:px-8 py-4 flex items-center justify-between">
		<a href="#" class="text-xl font-bold text-gray-900 tracking-[-0.03em]">
			Open<span class="text-[#0d9488]">Claw</span>
		</a>
		<div class="flex items-center gap-8">
			<a href="#how" class="text-[13px] font-medium text-gray-500 hover:text-gray-900 transition-colors hidden md:block">How It Works</a>
			<a href="#modules" class="text-[13px] font-medium text-gray-500 hover:text-gray-900 transition-colors hidden md:block">Modules</a>
			<a href="#pricing" class="text-[13px] font-medium text-gray-500 hover:text-gray-900 transition-colors hidden md:block">Pricing</a>
			<a href="#faq" class="text-[13px] font-medium text-gray-500 hover:text-gray-900 transition-colors hidden md:block">FAQ</a>
			<a
				href="#book"
				class="bg-gray-900 hover:bg-gray-800 text-white px-4 py-2 rounded-lg font-medium text-[13px] transition-all hover:shadow-lg"
			>
				Book a Call
			</a>
		</div>
	</div>
</nav>

<!-- Hero — asymmetric layout -->
<section class="min-h-[90vh] flex items-center pt-20 relative overflow-hidden">
	<!-- Dot grid background -->
	<div class="absolute inset-0 dot-grid opacity-[0.35]"></div>
	<!-- Gradient blob -->
	<div class="absolute top-20 right-[-10%] w-[500px] h-[500px] bg-gradient-to-br from-[#ccfbf1] via-[#99f6e4] to-transparent rounded-full blur-3xl opacity-40"></div>
	<div class="absolute bottom-0 left-0 w-full h-px bg-gradient-to-r from-transparent via-gray-300 to-transparent"></div>

	<div class="max-w-7xl mx-auto px-6 lg:px-8 py-20 relative grid lg:grid-cols-[1fr,0.85fr] gap-16 items-center">
		<!-- Left: Copy -->
		<div>
			<div class="inline-flex items-center gap-2 bg-[#0d9488]/[0.08] rounded-full px-3.5 py-1.5 mb-8">
				<span class="w-1.5 h-1.5 bg-[#0d9488] rounded-full animate-pulse"></span>
				<span class="text-[#0d9488] text-[13px] font-semibold tracking-wide uppercase">Private AI Infrastructure</span>
			</div>
			<h1 class="text-[clamp(2.5rem,5vw,4.25rem)] font-extrabold text-gray-900 leading-[1.08] tracking-[-0.04em] mb-6" style="text-wrap: balance;">
				Your AI Chief of Staff.
				<span class="bg-gradient-to-r from-[#0d9488] to-[#14b8a6] bg-clip-text text-transparent">Configured. Secured. Maintained.</span>
			</h1>
			<p class="text-lg text-gray-500 mb-10 max-w-xl leading-relaxed">
				We deploy private AI systems for founders, executives, and busy households.
				Your inbox triaged. Your calendar optimized. Your follow-ups tracked.
				Running 24/7 on your hardware. Owned by you.
			</p>
			<div class="flex flex-col sm:flex-row gap-3">
				<a
					href="#book"
					class="bg-gray-900 hover:bg-gray-800 text-white px-7 py-3.5 rounded-xl font-semibold text-[15px] transition-all text-center shadow-lg shadow-gray-900/10 hover:shadow-xl hover:shadow-gray-900/15 hover:-translate-y-0.5"
				>
					Book a Discovery Call
				</a>
				<a
					href="#how"
					class="border border-gray-300 hover:border-gray-400 text-gray-700 px-7 py-3.5 rounded-xl font-semibold text-[15px] transition-all text-center hover:-translate-y-0.5"
				>
					See How It Works
				</a>
			</div>
		</div>

		<!-- Right: Visual — mock briefing card -->
		<div class="hidden lg:block">
			<div class="relative">
				<!-- Shadow / depth layer -->
				<div class="absolute inset-0 bg-gradient-to-br from-[#0d9488]/10 to-transparent rounded-3xl translate-x-3 translate-y-3"></div>
				<!-- Main card -->
				<div class="relative bg-white border border-gray-200 rounded-2xl shadow-xl shadow-gray-200/60 overflow-hidden">
					<!-- Card header -->
					<div class="px-6 py-4 border-b border-gray-100 flex items-center justify-between">
						<div class="flex items-center gap-3">
							<div class="w-8 h-8 bg-[#0d9488]/10 rounded-lg flex items-center justify-center">
								<span class="text-[#0d9488] text-sm font-bold">OC</span>
							</div>
							<div>
								<div class="text-[13px] font-semibold text-gray-900">Daily Briefing</div>
								<div class="text-[11px] text-gray-400">Today at 6:00 AM</div>
							</div>
						</div>
						<div class="flex items-center gap-1.5">
							<div class="w-2.5 h-2.5 rounded-full bg-red-400"></div>
							<div class="w-2.5 h-2.5 rounded-full bg-amber-400"></div>
							<div class="w-2.5 h-2.5 rounded-full bg-green-400"></div>
						</div>
					</div>
					<!-- Card body -->
					<div class="p-6 space-y-4">
						<div class="flex items-start gap-3">
							<div class="w-7 h-7 bg-red-50 rounded-md flex items-center justify-center shrink-0 mt-0.5">
								<span class="text-red-500 text-xs font-bold">3</span>
							</div>
							<div>
								<div class="text-[13px] font-semibold text-gray-900">Urgent emails flagged</div>
								<div class="text-[12px] text-gray-400">Draft responses ready for review</div>
							</div>
						</div>
						<div class="flex items-start gap-3">
							<div class="w-7 h-7 bg-amber-50 rounded-md flex items-center justify-center shrink-0 mt-0.5">
								<span class="text-amber-600 text-xs font-bold">2</span>
							</div>
							<div>
								<div class="text-[13px] font-semibold text-gray-900">Calendar conflicts resolved</div>
								<div class="text-[12px] text-gray-400">Tuesday 2pm meeting moved to 3:30pm</div>
							</div>
						</div>
						<div class="flex items-start gap-3">
							<div class="w-7 h-7 bg-blue-50 rounded-md flex items-center justify-center shrink-0 mt-0.5">
								<span class="text-blue-500 text-xs font-bold">5</span>
							</div>
							<div>
								<div class="text-[13px] font-semibold text-gray-900">Follow-ups due today</div>
								<div class="text-[12px] text-gray-400">Including Board deck for Sarah — 3 days overdue</div>
							</div>
						</div>
						<div class="h-px bg-gray-100"></div>
						<div class="flex items-start gap-3">
							<div class="w-7 h-7 bg-[#0d9488]/10 rounded-md flex items-center justify-center shrink-0 mt-0.5">
								<span class="text-[#0d9488] text-xs">✓</span>
							</div>
							<div>
								<div class="text-[13px] font-semibold text-gray-900">12 emails auto-archived</div>
								<div class="text-[12px] text-gray-400">Newsletters, receipts, and notifications sorted</div>
							</div>
						</div>
					</div>
					<!-- Card footer -->
					<div class="px-6 py-3 bg-gray-50/80 border-t border-gray-100">
						<div class="text-[11px] text-gray-400 text-center">10 minutes to review · 87 minutes saved</div>
					</div>
				</div>
			</div>
		</div>
	</div>
</section>

<!-- Social proof strip -->
<section class="border-b border-gray-200 bg-white">
	<div class="max-w-7xl mx-auto px-6 lg:px-8 py-6 flex flex-wrap items-center justify-center gap-x-12 gap-y-3">
		{#each ['Client-owned infrastructure', 'No token markup', '14-day hypercare included', 'Live in under 2 weeks'] as item}
			<span class="flex items-center gap-2 text-[13px] text-gray-400 font-medium">
				<svg class="w-4 h-4 text-[#0d9488]" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2.5"><path stroke-linecap="round" stroke-linejoin="round" d="M5 13l4 4L19 7" /></svg>
				{item}
			</span>
		{/each}
	</div>
</section>

<!-- Problem -->
<section class="py-28 lg:py-32">
	<div class="max-w-7xl mx-auto px-6 lg:px-8">
		<div class="max-w-2xl mb-16">
			<p class="text-[13px] font-semibold text-[#0d9488] uppercase tracking-wider mb-3">The Problem</p>
			<h2 class="text-3xl md:text-[2.75rem] font-bold text-gray-900 leading-tight tracking-[-0.03em] mb-4" style="text-wrap: balance;">Sound Familiar?</h2>
			<p class="text-gray-500 text-lg">
				You're successful. But your day is consumed by operational noise.
			</p>
		</div>
		<div class="grid md:grid-cols-3 gap-6">
			<div class="group relative bg-white border border-gray-200 rounded-2xl p-8 hover:border-gray-300 hover:shadow-lg hover:shadow-gray-100 transition-all duration-300">
				<div class="absolute inset-x-0 top-0 h-1 bg-gradient-to-r from-red-400 to-red-300 rounded-t-2xl opacity-0 group-hover:opacity-100 transition-opacity"></div>
				<div class="w-12 h-12 bg-red-50 rounded-xl flex items-center justify-center mb-6">
					<span class="text-2xl">📧</span>
				</div>
				<h3 class="text-lg font-semibold text-gray-900 mb-3">Drowning in Email</h3>
				<p class="text-[15px] text-gray-500 leading-relaxed">
					47 unread before breakfast. Important messages buried under newsletters and noise.
					You spend 90+ minutes daily just triaging.
				</p>
			</div>
			<div class="group relative bg-white border border-gray-200 rounded-2xl p-8 hover:border-gray-300 hover:shadow-lg hover:shadow-gray-100 transition-all duration-300">
				<div class="absolute inset-x-0 top-0 h-1 bg-gradient-to-r from-amber-400 to-amber-300 rounded-t-2xl opacity-0 group-hover:opacity-100 transition-opacity"></div>
				<div class="w-12 h-12 bg-amber-50 rounded-xl flex items-center justify-center mb-6">
					<span class="text-2xl">📅</span>
				</div>
				<h3 class="text-lg font-semibold text-gray-900 mb-3">Calendar Chaos</h3>
				<p class="text-[15px] text-gray-500 leading-relaxed">
					Double-bookings. No buffer time. Scheduling conflicts you discover 5 minutes before the call.
					Your calendar runs you, not the other way around.
				</p>
			</div>
			<div class="group relative bg-white border border-gray-200 rounded-2xl p-8 hover:border-gray-300 hover:shadow-lg hover:shadow-gray-100 transition-all duration-300">
				<div class="absolute inset-x-0 top-0 h-1 bg-gradient-to-r from-blue-400 to-blue-300 rounded-t-2xl opacity-0 group-hover:opacity-100 transition-opacity"></div>
				<div class="w-12 h-12 bg-blue-50 rounded-xl flex items-center justify-center mb-6">
					<span class="text-2xl">🧠</span>
				</div>
				<h3 class="text-lg font-semibold text-gray-900 mb-3">Everything Slips Through</h3>
				<p class="text-[15px] text-gray-500 leading-relaxed">
					Follow-ups you forgot. Promises you made in meetings last month.
					The mental load of keeping track of everything is the real bottleneck.
				</p>
			</div>
		</div>
	</div>
</section>

<!-- Solution -->
<section class="py-28 lg:py-32 bg-white relative">
	<div class="absolute inset-0 dot-grid opacity-20"></div>
	<div class="max-w-7xl mx-auto px-6 lg:px-8 relative">
		<div class="max-w-2xl mb-16">
			<p class="text-[13px] font-semibold text-[#0d9488] uppercase tracking-wider mb-3">The Solution</p>
			<h2 class="text-3xl md:text-[2.75rem] font-bold text-gray-900 leading-tight tracking-[-0.03em] mb-4" style="text-wrap: balance;">What You Wake Up To Instead</h2>
			<p class="text-gray-500 text-lg">
				Your AI Chief of Staff handles the operational noise so you can focus on what matters.
			</p>
		</div>
		<div class="gradient-border rounded-2xl bg-white max-w-4xl">
			<div class="p-8 md:p-12">
				<div class="space-y-8">
					{#each [
						{ n: '01', title: 'Inbox Triaged & Prioritized', desc: '3 emails flagged as urgent with draft responses ready. 12 emails categorized as FYI-only and archived. Zero noise.' },
						{ n: '02', title: 'Calendar Optimized', desc: 'Conflicts resolved. Travel time added. Buffer periods protected. Your day structured for peak performance.' },
						{ n: '03', title: 'Daily Briefing at 6am', desc: "Today's priorities, pending follow-ups with context from previous conversations, and key metrics — all in one place." },
						{ n: '04', title: 'Follow-ups Tracked Automatically', desc: 'Every commitment logged. Every promise remembered. Nothing falls through the cracks because your AI never forgets.' },
						{ n: '05', title: 'Research On Demand', desc: 'Ask a question in plain English. Get a researched answer with sources. Competitive analysis, market data, or prep for your next meeting.' }
					] as item}
						<div class="flex items-start gap-6 group">
							<div class="text-[2rem] font-black text-gray-200 group-hover:text-[#0d9488]/30 transition-colors leading-none tracking-[-0.05em] shrink-0 w-12">{item.n}</div>
							<div>
								<h3 class="text-[15px] font-semibold text-gray-900 mb-1">{item.title}</h3>
								<p class="text-[15px] text-gray-500 leading-relaxed">{item.desc}</p>
							</div>
						</div>
					{/each}
				</div>
				<div class="mt-10 pt-8 border-t border-gray-100 flex items-center justify-between flex-wrap gap-4">
					<p class="text-gray-500 text-[15px]">
						<span class="text-gray-900 font-semibold">10 minutes reviewing</span> instead of <span class="text-gray-900 font-semibold">90 minutes drowning.</span>
					</p>
					<a href="#book" class="text-[#0d9488] text-[13px] font-semibold hover:underline underline-offset-4">See how it works →</a>
				</div>
			</div>
		</div>
	</div>
</section>

<!-- How It Works -->
<section id="how" class="py-28 lg:py-32">
	<div class="max-w-7xl mx-auto px-6 lg:px-8">
		<div class="max-w-2xl mb-20">
			<p class="text-[13px] font-semibold text-[#0d9488] uppercase tracking-wider mb-3">Process</p>
			<h2 class="text-3xl md:text-[2.75rem] font-bold text-gray-900 leading-tight tracking-[-0.03em] mb-4">How It Works</h2>
			<p class="text-gray-500 text-lg">
				From first call to live system in under two weeks.
			</p>
		</div>
		<div class="grid md:grid-cols-3 gap-16">
			{#each [
				{ n: '01', title: 'Discover', desc: "30-minute call. We learn your workflow, tools, and priorities. You tell us what eats your time. We design the system." },
				{ n: '02', title: 'Deploy', desc: 'We configure your private AI infrastructure. Integrations connected. Security hardened. Workflows tested with your real data.' },
				{ n: '03', title: 'Optimize', desc: "14-day hypercare. We fine-tune based on how you actually use it. Then ongoing managed care to keep everything running perfectly." }
			] as step}
				<div class="relative">
					<div class="text-[5rem] font-black text-gray-100 leading-none tracking-[-0.05em] mb-4">{step.n}</div>
					<h3 class="text-xl font-semibold text-gray-900 mb-3">{step.title}</h3>
					<p class="text-[15px] text-gray-500 leading-relaxed">{step.desc}</p>
				</div>
			{/each}
		</div>
	</div>
</section>

<!-- Modules -->
<section id="modules" class="py-28 lg:py-32 bg-white">
	<div class="max-w-7xl mx-auto px-6 lg:px-8">
		<div class="max-w-2xl mb-16">
			<p class="text-[13px] font-semibold text-[#0d9488] uppercase tracking-wider mb-3">Modules</p>
			<h2 class="text-3xl md:text-[2.75rem] font-bold text-gray-900 leading-tight tracking-[-0.03em] mb-4" style="text-wrap: balance;">Expansion Modules</h2>
			<p class="text-gray-500 text-lg">
				Start with the AI Chief of Staff base. Add modules based on your identity and needs.
			</p>
		</div>
		<div class="grid md:grid-cols-2 gap-5">
			{#each modules as mod}
				<div class="group relative bg-[#fbfcfd] border border-gray-200 rounded-2xl p-7 hover:border-[#0d9488]/40 hover:shadow-lg hover:shadow-[#0d9488]/5 transition-all duration-300">
					<div class="flex items-center gap-4 mb-5">
						<div class="w-11 h-11 bg-[#0d9488]/[0.07] group-hover:bg-[#0d9488]/[0.12] rounded-xl flex items-center justify-center transition-colors">
							<span class="text-xl">{mod.icon}</span>
						</div>
						<div>
							<h3 class="text-[15px] font-semibold text-gray-900">{mod.name}</h3>
							<p class="text-[#0d9488] text-[12px] font-semibold tracking-wide">{mod.audience}</p>
						</div>
					</div>
					<ul class="space-y-2 mb-5">
						{#each mod.features as feat}
							<li class="flex items-center gap-2.5 text-[14px] text-gray-500">
								<svg class="w-3.5 h-3.5 text-[#0d9488] shrink-0" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="3"><path stroke-linecap="round" stroke-linejoin="round" d="M5 13l4 4L19 7" /></svg>
								{feat}
							</li>
						{/each}
					</ul>
					<div class="text-[13px] font-semibold text-gray-400">{mod.price}</div>
				</div>
			{/each}
		</div>
	</div>
</section>

<!-- Pricing -->
<section id="pricing" class="py-28 lg:py-32 relative">
	<div class="absolute inset-0 dot-grid opacity-20"></div>
	<div class="max-w-7xl mx-auto px-6 lg:px-8 relative">
		<div class="text-center mb-16">
			<p class="text-[13px] font-semibold text-[#0d9488] uppercase tracking-wider mb-3">Pricing</p>
			<h2 class="text-3xl md:text-[2.75rem] font-bold text-gray-900 leading-tight tracking-[-0.03em] mb-4">Investment</h2>
			<p class="text-gray-500 text-lg max-w-xl mx-auto">
				Less than a part-time executive assistant. Available 24/7.
			</p>
		</div>
		<div class="grid md:grid-cols-3 gap-6 max-w-5xl mx-auto">
			<!-- Good -->
			<div class="bg-white border border-gray-200 rounded-2xl p-7 hover:shadow-lg hover:shadow-gray-100 transition-all duration-300">
				<div class="mb-6">
					<h3 class="text-[15px] font-semibold text-gray-900 mb-0.5">AI Chief of Staff</h3>
					<p class="text-[12px] text-gray-400 font-medium">The foundation</p>
				</div>
				<div class="mb-1">
					<span class="text-4xl font-bold text-gray-900 tracking-[-0.03em]">$2,500</span>
					<span class="text-gray-400 text-sm"> setup</span>
				</div>
				<div class="mb-8">
					<span class="text-2xl font-bold text-gray-900 tracking-[-0.02em]">$1,500</span>
					<span class="text-gray-400 text-sm">/month</span>
				</div>
				<ul class="space-y-3 mb-8">
					{#each ['Inbox prioritization & drafting', 'Calendar intelligence', 'Daily & weekly briefings', 'Follow-up tracking', 'Research assistance', 'Security hardening', '14-day hypercare'] as f}
						<li class="flex items-start gap-2.5 text-gray-500 text-[13px]">
							<svg class="w-3.5 h-3.5 text-[#0d9488] shrink-0 mt-0.5" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="3"><path stroke-linecap="round" stroke-linejoin="round" d="M5 13l4 4L19 7" /></svg>
							{f}
						</li>
					{/each}
				</ul>
				<a href="#book" class="block text-center border border-gray-300 hover:border-gray-400 text-gray-700 py-3 rounded-xl font-semibold text-[13px] transition-all hover:shadow-sm">
					Get Started
				</a>
			</div>

			<!-- Better -->
			<div class="bg-white border-2 border-gray-900 rounded-2xl p-7 relative shadow-xl shadow-gray-200/60">
				<div class="absolute -top-3 left-1/2 -translate-x-1/2 bg-gray-900 text-white text-[11px] font-bold px-3.5 py-1 rounded-full tracking-wide">
					MOST POPULAR
				</div>
				<div class="mb-6">
					<h3 class="text-[15px] font-semibold text-gray-900 mb-0.5">Chief of Staff + Module</h3>
					<p class="text-[12px] text-gray-400 font-medium">Best value</p>
				</div>
				<div class="mb-1">
					<span class="text-4xl font-bold text-gray-900 tracking-[-0.03em]">$2,500</span>
					<span class="text-gray-400 text-sm"> setup</span>
				</div>
				<div class="mb-8">
					<span class="text-2xl font-bold text-gray-900 tracking-[-0.02em]">$2,500–$3,000</span>
					<span class="text-gray-400 text-sm">/mo</span>
				</div>
				<ul class="space-y-3 mb-8">
					{#each ['Everything in base', '1 expansion module of your choice', 'Custom workflow configuration', 'Monthly optimization calls', 'Priority support channel'] as f}
						<li class="flex items-start gap-2.5 text-gray-500 text-[13px]">
							<svg class="w-3.5 h-3.5 text-[#0d9488] shrink-0 mt-0.5" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="3"><path stroke-linecap="round" stroke-linejoin="round" d="M5 13l4 4L19 7" /></svg>
							{#if f.includes('expansion')}<strong class="text-gray-900">{f}</strong>{:else}{f}{/if}
						</li>
					{/each}
				</ul>
				<a href="#book" class="block text-center bg-gray-900 hover:bg-gray-800 text-white py-3 rounded-xl font-semibold text-[13px] transition-all hover:shadow-lg">
					Book a Call
				</a>
			</div>

			<!-- Best -->
			<div class="bg-white border border-gray-200 rounded-2xl p-7 hover:shadow-lg hover:shadow-gray-100 transition-all duration-300">
				<div class="mb-6">
					<h3 class="text-[15px] font-semibold text-gray-900 mb-0.5">Full Suite</h3>
					<p class="text-[12px] text-gray-400 font-medium">Maximum leverage</p>
				</div>
				<div class="mb-1">
					<span class="text-4xl font-bold text-gray-900 tracking-[-0.03em]">$5,000</span>
					<span class="text-gray-400 text-sm"> setup</span>
				</div>
				<div class="mb-8">
					<span class="text-2xl font-bold text-gray-900 tracking-[-0.02em]">$4,000–$5,000</span>
					<span class="text-gray-400 text-sm">/mo</span>
				</div>
				<ul class="space-y-3 mb-8">
					{#each ['Everything in base', '2–3 expansion modules', 'Advanced workflow automation', 'Dedicated support channel', 'Quarterly security reviews', 'White-glove onboarding'] as f}
						<li class="flex items-start gap-2.5 text-gray-500 text-[13px]">
							<svg class="w-3.5 h-3.5 text-[#0d9488] shrink-0 mt-0.5" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="3"><path stroke-linecap="round" stroke-linejoin="round" d="M5 13l4 4L19 7" /></svg>
							{#if f.includes('expansion')}<strong class="text-gray-900">{f}</strong>{:else}{f}{/if}
						</li>
					{/each}
				</ul>
				<a href="#book" class="block text-center border border-gray-300 hover:border-gray-400 text-gray-700 py-3 rounded-xl font-semibold text-[13px] transition-all hover:shadow-sm">
					Contact Us
				</a>
			</div>
		</div>
		<p class="text-center text-gray-400 text-[13px] mt-8">
			You pay AI providers (Anthropic, OpenAI) directly. We never mark up token costs.
		</p>
	</div>
</section>

<!-- Trust -->
<section class="py-28 lg:py-32 bg-white">
	<div class="max-w-7xl mx-auto px-6 lg:px-8">
		<div class="text-center mb-16">
			<p class="text-[13px] font-semibold text-[#0d9488] uppercase tracking-wider mb-3">Why Us</p>
			<h2 class="text-3xl md:text-[2.75rem] font-bold text-gray-900 leading-tight tracking-[-0.03em]">Why OpenClaw</h2>
		</div>
		<div class="grid md:grid-cols-2 lg:grid-cols-4 gap-6">
			{#each [
				{ icon: '🔒', title: 'You Own Everything', desc: 'Your hardware. Your API keys. Your data. No vendor lock-in.' },
				{ icon: '💰', title: 'No Token Markup', desc: 'Pay AI providers directly at their standard rates. We charge for architecture, not compute.' },
				{ icon: '🛡️', title: 'Security First', desc: 'Hardened deployment. Encrypted credentials. Audit trails. Your data never touches our servers.' },
				{ icon: '🧩', title: 'Modular by Design', desc: "Start with what you need. Add modules as you grow. No paying for features you don't use." }
			] as item}
				<div class="text-center p-8 rounded-2xl border border-transparent hover:border-gray-200 hover:bg-[#fbfcfd] transition-all duration-300">
					<div class="w-12 h-12 bg-gray-100 rounded-xl flex items-center justify-center mx-auto mb-5">
						<span class="text-xl">{item.icon}</span>
					</div>
					<h3 class="text-gray-900 text-[15px] font-semibold mb-2">{item.title}</h3>
					<p class="text-gray-500 text-[14px] leading-relaxed">{item.desc}</p>
				</div>
			{/each}
		</div>
	</div>
</section>

<!-- FAQ -->
<section id="faq" class="py-28 lg:py-32">
	<div class="max-w-2xl mx-auto px-6 lg:px-8">
		<div class="mb-16">
			<p class="text-[13px] font-semibold text-[#0d9488] uppercase tracking-wider mb-3">FAQ</p>
			<h2 class="text-3xl md:text-[2.75rem] font-bold text-gray-900 leading-tight tracking-[-0.03em]">Questions</h2>
		</div>
		<div class="space-y-3">
			{#each faqs as faq, i}
				<button
					class="w-full text-left bg-white border border-gray-200 rounded-xl px-6 py-5 hover:border-gray-300 transition-all duration-200 {openFaq === i ? 'shadow-sm' : ''}"
					onclick={() => toggleFaq(i)}
				>
					<div class="flex items-center justify-between gap-4">
						<h3 class="text-[15px] text-gray-900 font-semibold">{faq.q}</h3>
						<div class="w-6 h-6 rounded-md bg-gray-100 flex items-center justify-center shrink-0">
							<svg class="w-3.5 h-3.5 text-gray-500 transition-transform duration-200 {openFaq === i ? 'rotate-180' : ''}" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2.5">
								<path stroke-linecap="round" stroke-linejoin="round" d="M19 9l-7 7-7-7" />
							</svg>
						</div>
					</div>
					{#if openFaq === i}
						<p class="text-[14px] text-gray-500 mt-3 leading-relaxed">{faq.a}</p>
					{/if}
				</button>
			{/each}
		</div>
	</div>
</section>

<!-- Final CTA -->
<section id="book" class="py-28 lg:py-32 bg-gray-900 relative overflow-hidden">
	<!-- Decorative circles -->
	<div class="absolute top-10 right-10 w-64 h-64 border border-white/5 rounded-full"></div>
	<div class="absolute bottom-10 left-10 w-40 h-40 border border-white/5 rounded-full"></div>
	<div class="absolute top-1/2 left-1/3 -translate-y-1/2 w-96 h-96 bg-[#0d9488]/10 rounded-full blur-3xl"></div>

	<div class="max-w-2xl mx-auto px-6 lg:px-8 text-center relative">
		<h2 class="text-3xl md:text-4xl font-bold text-white mb-6 tracking-[-0.03em]">
			Ready to Get Your Time Back?
		</h2>
		<p class="text-gray-400 text-lg mb-10 max-w-xl mx-auto leading-relaxed">
			Book a 30-minute discovery call. We'll learn your workflow and show you exactly how
			your AI Chief of Staff would work. No commitment. No pitch deck. Just a conversation.
		</p>
		<div class="flex flex-col sm:flex-row gap-3 justify-center">
			<a
				href="https://calendly.com"
				target="_blank"
				rel="noopener noreferrer"
				class="inline-block bg-white hover:bg-gray-100 text-gray-900 px-8 py-4 rounded-xl font-semibold text-[15px] transition-all shadow-lg hover:shadow-xl hover:-translate-y-0.5"
			>
				Book Your Discovery Call
			</a>
			<a
				href="#how"
				class="inline-block border border-white/20 hover:border-white/40 text-white px-8 py-4 rounded-xl font-semibold text-[15px] transition-all hover:-translate-y-0.5"
			>
				Learn More
			</a>
		</div>
		<p class="text-gray-600 text-[13px] mt-8">Currently accepting a limited number of new clients.</p>
	</div>
</section>

<!-- Footer -->
<footer class="bg-gray-900 border-t border-white/5 py-10">
	<div class="max-w-7xl mx-auto px-6 lg:px-8">
		<div class="flex flex-col md:flex-row items-center justify-between gap-4">
			<div class="text-white font-bold text-lg tracking-[-0.02em]">
				Open<span class="text-[#14b8a6]">Claw</span>
			</div>
			<p class="text-gray-500 text-[13px]">
				We sell architecture and leverage, not compute.
			</p>
			<p class="text-gray-600 text-[13px]">
				&copy; {new Date().getFullYear()} OpenClaw. All rights reserved.
			</p>
		</div>
	</div>
</footer>
