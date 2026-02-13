<script lang="ts">
	const modules = [
		{
			icon: '⚡',
			name: 'Operator System',
			audience: 'For Founders & Execs',
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
			q: "Wait — how is this different from ChatGPT?",
			a: "Great question. ChatGPT is a chat window you open when you remember to. Your OpenClaw system is infrastructure. It runs 24/7, connected to your email, calendar, CRM, and tools. It doesn't wait for you to ask — it triages your inbox at 6am, drafts responses, flags urgent items, and tracks your follow-ups automatically. You wake up to a briefing, not a backlog."
		},
		{
			q: 'Do I need to be technical?',
			a: "Nope. We handle everything — deployment, security, integrations, maintenance, all of it. You talk to your AI the way you'd talk to a real chief of staff: over email, Slack, or text. If you can send a message, you can use OpenClaw."
		},
		{
			q: 'Who owns the AI and the data?',
			a: "You do. 100%. Your system runs on your infrastructure, uses your API keys, and your data never touches our servers. If you ever want to part ways, you keep everything. No hostage situations."
		},
		{
			q: 'What AI models do you use?',
			a: "We configure your system with the best models for each task — Claude, GPT, Gemini, whatever fits. You pay the AI providers directly at their rates. We never mark up tokens. We make money on the architecture, not the compute."
		},
		{
			q: 'How long until I\'m up and running?',
			a: "Most deployments are live within 5–7 business days. That includes a discovery call, configuration, integration setup, testing, and a 14-day hypercare period where we fine-tune everything based on how you actually work."
		},
		{
			q: 'Can I start small and add more later?',
			a: "That's literally how we designed it. Most clients start with the base AI Chief of Staff, see the value, then bolt on modules as they need them. No long-term contracts. Scale up, scale down, whatever makes sense."
		}
	];

	let openFaq = $state<number | null>(null);

	function toggleFaq(i: number) {
		openFaq = openFaq === i ? null : i;
	}
</script>

<!-- Nav -->
<nav class="fixed top-0 w-full z-50 bg-[#0f1117]/95 backdrop-blur-sm border-b border-white/5">
	<div class="max-w-6xl mx-auto px-6 py-4 flex items-center justify-between">
		<div class="text-xl font-bold text-white tracking-tight">
			Open<span class="text-[#f97316]">Claw</span>
		</div>
		<a
			href="#book"
			class="bg-[#f97316] hover:bg-[#fb923c] text-white px-5 py-2.5 rounded-lg font-semibold text-sm transition-colors"
		>
			Let's Talk
		</a>
	</div>
</nav>

<!-- Hero -->
<section class="min-h-screen flex items-center bg-[#0f1117] pt-20 relative overflow-hidden">
	<!-- Subtle gradient glow -->
	<div class="absolute top-1/4 -right-1/4 w-[600px] h-[600px] bg-[#f97316]/5 rounded-full blur-3xl"></div>
	<div class="absolute bottom-0 left-0 w-full h-px bg-gradient-to-r from-transparent via-[#f97316]/20 to-transparent"></div>
	<div class="max-w-6xl mx-auto px-6 py-20 relative">
		<div class="max-w-3xl">
			<div class="inline-block bg-[#f97316]/10 border border-[#f97316]/20 rounded-full px-4 py-1.5 text-[#f97316] text-sm font-medium mb-8">
				Private AI Infrastructure — Built for You
			</div>
			<h1 class="text-5xl md:text-6xl lg:text-7xl font-black text-white leading-[1.05] mb-6">
				Stop drowning in your
				<span class="text-[#f97316] block mt-1">own success.</span>
			</h1>
			<p class="text-xl text-gray-400 mb-4 max-w-2xl leading-relaxed">
				You built something great. Now you spend your days buried in email, chasing follow-ups, and managing a calendar that manages you.
			</p>
			<p class="text-xl text-white/90 mb-10 max-w-2xl leading-relaxed font-medium">
				We deploy AI systems that actually handle that stuff — running 24/7 on <em>your</em> hardware, owned by <em>you</em>.
			</p>
			<div class="flex flex-col sm:flex-row gap-4">
				<a
					href="#book"
					class="bg-[#f97316] hover:bg-[#fb923c] text-white px-8 py-4 rounded-lg font-bold text-lg transition-colors text-center shadow-lg shadow-[#f97316]/20"
				>
					Book a Discovery Call
				</a>
				<a
					href="#how"
					class="border border-white/20 hover:border-white/40 text-white px-8 py-4 rounded-lg font-semibold text-lg transition-colors text-center"
				>
					How It Works
				</a>
			</div>
			<div class="mt-14 flex flex-wrap items-center gap-8 text-sm text-gray-500">
				<span class="flex items-center gap-2">
					<span class="w-2 h-2 bg-green-500 rounded-full animate-pulse"></span>
					Your infrastructure. Your data.
				</span>
				<span class="flex items-center gap-2">
					<span class="w-2 h-2 bg-green-500 rounded-full animate-pulse"></span>
					Zero token markup
				</span>
				<span class="flex items-center gap-2">
					<span class="w-2 h-2 bg-green-500 rounded-full animate-pulse"></span>
					Live in under 2 weeks
				</span>
			</div>
		</div>
	</div>
</section>

<!-- Problem -->
<section class="bg-[#1a1d27] py-24">
	<div class="max-w-6xl mx-auto px-6">
		<div class="text-center mb-16">
			<h2 class="text-3xl md:text-4xl font-bold text-white mb-4">Be honest. How many of these are you?</h2>
		</div>
		<div class="grid md:grid-cols-3 gap-8">
			<div class="bg-[#0f1117]/60 border border-white/5 rounded-2xl p-8 hover:border-[#f97316]/20 transition-colors">
				<div class="text-4xl mb-4">📧</div>
				<h3 class="text-xl font-bold text-white mb-3">The Inbox Trap</h3>
				<p class="text-gray-400 leading-relaxed">
					47 unread before breakfast. Important stuff buried under newsletters and noise.
					You spend 90+ minutes <em>just triaging</em> before you do any real work.
				</p>
			</div>
			<div class="bg-[#0f1117]/60 border border-white/5 rounded-2xl p-8 hover:border-[#f97316]/20 transition-colors">
				<div class="text-4xl mb-4">📅</div>
				<h3 class="text-xl font-bold text-white mb-3">Calendar Tetris</h3>
				<p class="text-gray-400 leading-relaxed">
					Double-bookings. Zero buffer time. You find out about conflicts 5 minutes before the call.
					Your calendar runs <em>you</em>. Not the other way around.
				</p>
			</div>
			<div class="bg-[#0f1117]/60 border border-white/5 rounded-2xl p-8 hover:border-[#f97316]/20 transition-colors">
				<div class="text-4xl mb-4">🧠</div>
				<h3 class="text-xl font-bold text-white mb-3">The Mental Load</h3>
				<p class="text-gray-400 leading-relaxed">
					Follow-ups you forgot. Promises from last month's meeting.
					That constant low-grade anxiety that something important is slipping through the cracks.
				</p>
			</div>
		</div>
		<p class="text-center text-gray-500 mt-12 text-lg">
			Yeah. We've been there too. That's why we built this.
		</p>
	</div>
</section>

<!-- Solution / What You Get -->
<section class="bg-[#0f1117] py-24">
	<div class="max-w-6xl mx-auto px-6">
		<div class="text-center mb-16">
			<h2 class="text-3xl md:text-4xl font-bold text-white mb-4">Here's what your morning looks like instead</h2>
			<p class="text-gray-400 text-lg max-w-2xl mx-auto">
				You wake up. Your AI Chief of Staff already handled the noise. You just review.
			</p>
		</div>
		<div class="bg-[#1a1d27] border border-white/10 rounded-2xl p-8 md:p-12 max-w-4xl mx-auto">
			<div class="space-y-6">
				{#each [
					{ n: '1', title: 'Inbox: Triaged & Prioritized', desc: '3 emails flagged urgent with draft responses ready. 12 categorized as FYI and archived. The rest? Handled. Zero noise hitting your eyes.' },
					{ n: '2', title: 'Calendar: Actually Makes Sense', desc: 'Conflicts resolved. Travel time added. Buffer periods protected. Your day is structured before you even open the app.' },
					{ n: '3', title: 'Daily Briefing: Waiting for You at 6am', desc: "Today's priorities. Pending follow-ups with full context from previous conversations. Key metrics. All in one place — like a real chief of staff prepped it." },
					{ n: '4', title: 'Follow-ups: Nothing Falls Through', desc: 'Every commitment logged. Every promise remembered. Your AI doesn\'t forget the thing you said you\'d do in Tuesday\'s meeting.' },
					{ n: '5', title: 'Research: Ask and Receive', desc: 'Need competitive intel before your 2pm? Market data for a pitch? Just ask in plain English. Get a researched answer with sources, not a chatbot response.' }
				] as item}
					<div class="flex items-start gap-4">
						<div class="w-10 h-10 bg-[#f97316]/15 rounded-lg flex items-center justify-center shrink-0 text-[#f97316] font-bold">{item.n}</div>
						<div>
							<h3 class="text-lg font-bold text-white">{item.title}</h3>
							<p class="text-gray-400">{item.desc}</p>
						</div>
					</div>
				{/each}
			</div>
			<div class="mt-10 pt-8 border-t border-white/10 text-center">
				<p class="text-xl">
					<span class="text-white font-bold">10 minutes reviewing.</span>
					<span class="text-gray-500"> Instead of 90 minutes drowning.</span>
				</p>
			</div>
		</div>
	</div>
</section>

<!-- How It Works -->
<section id="how" class="bg-[#1a1d27] py-24">
	<div class="max-w-6xl mx-auto px-6">
		<div class="text-center mb-16">
			<h2 class="text-3xl md:text-4xl font-bold text-white mb-4">Three steps. Two weeks. Done.</h2>
			<p class="text-gray-400 text-lg max-w-2xl mx-auto">
				We've done this enough times to make it painless.
			</p>
		</div>
		<div class="grid md:grid-cols-3 gap-8">
			{#each [
				{ n: '01', title: 'Discover', desc: "30-minute call. You tell us what eats your time — we figure out how to kill it. No sales pitch. Just a conversation about your workflow." },
				{ n: '02', title: 'Deploy', desc: 'We configure your private AI system. Connect your tools. Harden security. Test everything with your real data. You don\'t touch a terminal.' },
				{ n: '03', title: 'Optimize', desc: "14 days of hypercare. We watch how you use it, fine-tune the workflows, and make sure it actually fits your life. Then ongoing managed care keeps it sharp." }
			] as step}
				<div class="text-center">
					<div class="text-5xl font-black text-[#f97316]/20 mb-4">{step.n}</div>
					<h3 class="text-xl font-bold text-white mb-3">{step.title}</h3>
					<p class="text-gray-400 leading-relaxed">{step.desc}</p>
				</div>
			{/each}
		</div>
	</div>
</section>

<!-- Modules -->
<section class="bg-[#0f1117] py-24">
	<div class="max-w-6xl mx-auto px-6">
		<div class="text-center mb-6">
			<h2 class="text-3xl md:text-4xl font-bold text-white mb-4">Bolt on what you need. Ignore the rest.</h2>
			<p class="text-gray-400 text-lg max-w-2xl mx-auto">
				Everyone starts with the AI Chief of Staff base. Then you choose your own adventure.
			</p>
		</div>
		<div class="grid md:grid-cols-2 gap-8 mt-12">
			{#each modules as mod}
				<div class="bg-[#1a1d27] border border-white/10 rounded-2xl p-8 hover:border-[#f97316]/30 transition-colors group">
					<div class="flex items-center gap-3 mb-4">
						<span class="text-3xl">{mod.icon}</span>
						<div>
							<h3 class="text-xl font-bold text-white">{mod.name}</h3>
							<p class="text-[#f97316] text-sm font-medium">{mod.audience}</p>
						</div>
					</div>
					<ul class="space-y-2 mb-6">
						{#each mod.features as feat}
							<li class="flex items-center gap-2 text-gray-400">
								<span class="text-[#f97316] text-sm">&#10003;</span>
								{feat}
							</li>
						{/each}
					</ul>
					<div class="text-[#f59e0b] font-semibold text-sm">{mod.price}</div>
				</div>
			{/each}
		</div>
	</div>
</section>

<!-- Pricing -->
<section class="bg-[#1a1d27] py-24">
	<div class="max-w-6xl mx-auto px-6">
		<div class="text-center mb-16">
			<h2 class="text-3xl md:text-4xl font-bold text-white mb-4">Straightforward pricing. No surprises.</h2>
			<p class="text-gray-400 text-lg max-w-2xl mx-auto">
				Cheaper than a part-time EA. Runs 24/7. Never calls in sick.
			</p>
		</div>
		<div class="grid md:grid-cols-3 gap-8 max-w-5xl mx-auto">
			<!-- Good -->
			<div class="bg-[#0f1117] border border-white/10 rounded-2xl p-8">
				<h3 class="text-lg font-bold text-white mb-1">AI Chief of Staff</h3>
				<p class="text-gray-500 text-sm mb-6">The foundation</p>
				<div class="mb-2">
					<span class="text-4xl font-black text-white">$2,500</span>
					<span class="text-gray-400"> setup</span>
				</div>
				<div class="mb-8">
					<span class="text-2xl font-bold text-white">$1,500</span>
					<span class="text-gray-400">/month</span>
				</div>
				<ul class="space-y-3 mb-8">
					{#each ['Inbox prioritization & drafting', 'Calendar intelligence', 'Daily & weekly briefings', 'Follow-up tracking', 'Research on demand', 'Security hardening', '14-day hypercare'] as f}
						<li class="flex items-start gap-2 text-gray-400 text-sm">
							<span class="text-[#f97316] mt-0.5">&#10003;</span>{f}
						</li>
					{/each}
				</ul>
				<a href="#book" class="block text-center border border-white/20 hover:border-white/40 text-white py-3 rounded-lg font-semibold transition-colors">
					Get Started
				</a>
			</div>

			<!-- Better -->
			<div class="bg-[#0f1117] border-2 border-[#f97316] rounded-2xl p-8 relative shadow-lg shadow-[#f97316]/10">
				<div class="absolute -top-3 left-1/2 -translate-x-1/2 bg-[#f97316] text-white text-xs font-bold px-4 py-1 rounded-full">
					MOST POPULAR
				</div>
				<h3 class="text-lg font-bold text-white mb-1">Chief of Staff + Module</h3>
				<p class="text-gray-500 text-sm mb-6">Best value</p>
				<div class="mb-2">
					<span class="text-4xl font-black text-white">$2,500</span>
					<span class="text-gray-400"> setup</span>
				</div>
				<div class="mb-8">
					<span class="text-2xl font-bold text-white">$2,500–$3,000</span>
					<span class="text-gray-400">/mo</span>
				</div>
				<ul class="space-y-3 mb-8">
					{#each ['Everything in base', '1 expansion module of your choice', 'Custom workflow config', 'Monthly optimization calls', 'Priority support'] as f}
						<li class="flex items-start gap-2 text-gray-400 text-sm">
							<span class="text-[#f97316] mt-0.5">&#10003;</span>
							{#if f.includes('expansion')}<strong class="text-white">{f}</strong>{:else}{f}{/if}
						</li>
					{/each}
				</ul>
				<a href="#book" class="block text-center bg-[#f97316] hover:bg-[#fb923c] text-white py-3 rounded-lg font-bold transition-colors">
					Book a Call
				</a>
			</div>

			<!-- Best -->
			<div class="bg-[#0f1117] border border-[#f59e0b]/30 rounded-2xl p-8">
				<h3 class="text-lg font-bold text-white mb-1">Full Suite</h3>
				<p class="text-gray-500 text-sm mb-6">The whole enchilada</p>
				<div class="mb-2">
					<span class="text-4xl font-black text-white">$5,000</span>
					<span class="text-gray-400"> setup</span>
				</div>
				<div class="mb-8">
					<span class="text-2xl font-bold text-white">$4,000–$5,000</span>
					<span class="text-gray-400">/mo</span>
				</div>
				<ul class="space-y-3 mb-8">
					{#each ['Everything in base', '2–3 expansion modules', 'Advanced workflow automation', 'Dedicated support channel', 'Quarterly security reviews', 'White-glove onboarding'] as f}
						<li class="flex items-start gap-2 text-gray-400 text-sm">
							<span class="text-[#f97316] mt-0.5">&#10003;</span>
							{#if f.includes('expansion')}<strong class="text-white">{f}</strong>{:else}{f}{/if}
						</li>
					{/each}
				</ul>
				<a href="#book" class="block text-center border border-[#f59e0b]/40 hover:border-[#f59e0b] text-[#f59e0b] py-3 rounded-lg font-semibold transition-colors">
					Let's Talk
				</a>
			</div>
		</div>
		<p class="text-center text-gray-500 text-sm mt-8">
			You pay AI providers (Anthropic, OpenAI) directly. We never mark up token costs. Ever.
		</p>
	</div>
</section>

<!-- Trust -->
<section class="bg-[#0f1117] py-24">
	<div class="max-w-6xl mx-auto px-6">
		<div class="text-center mb-16">
			<h2 class="text-3xl md:text-4xl font-bold text-white mb-4">Why people trust us with their operations</h2>
		</div>
		<div class="grid md:grid-cols-2 lg:grid-cols-4 gap-6">
			{#each [
				{ icon: '🔒', title: 'You Own Everything', desc: "Your hardware. Your API keys. Your data. We build it, you own it. Walk away anytime — it's all yours." },
				{ icon: '💰', title: 'No Token Markup', desc: "Pay AI providers directly at their rates. We make money on architecture, not compute. That's how it should be." },
				{ icon: '🛡️', title: 'Security First', desc: 'Hardened deployment. Encrypted credentials. Audit trails. Your data never touches our servers. Period.' },
				{ icon: '🧩', title: 'Start Small, Go Big', desc: "Begin with what you need today. Add modules tomorrow. No paying for features you'll never use." }
			] as item}
				<div class="text-center p-6 rounded-2xl hover:bg-[#1a1d27]/50 transition-colors">
					<div class="text-3xl mb-4">{item.icon}</div>
					<h3 class="text-white font-bold mb-2">{item.title}</h3>
					<p class="text-gray-400 text-sm leading-relaxed">{item.desc}</p>
				</div>
			{/each}
		</div>
	</div>
</section>

<!-- FAQ -->
<section class="bg-[#1a1d27] py-24">
	<div class="max-w-3xl mx-auto px-6">
		<div class="text-center mb-16">
			<h2 class="text-3xl md:text-4xl font-bold text-white mb-4">Got questions? Good.</h2>
		</div>
		<div class="space-y-4">
			{#each faqs as faq, i}
				<button
					class="w-full text-left bg-[#0f1117] border border-white/10 rounded-xl p-6 hover:border-[#f97316]/30 transition-colors"
					onclick={() => toggleFaq(i)}
				>
					<div class="flex items-center justify-between">
						<h3 class="text-white font-semibold pr-4">{faq.q}</h3>
						<span class="text-[#f97316] text-xl shrink-0 transition-transform" class:rotate-45={openFaq === i}>{openFaq === i ? '−' : '+'}</span>
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
<section id="book" class="bg-[#0f1117] py-24 relative overflow-hidden">
	<div class="absolute inset-0 bg-gradient-to-b from-[#1a1d27] to-[#0f1117]"></div>
	<div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 w-[500px] h-[500px] bg-[#f97316]/5 rounded-full blur-3xl"></div>
	<div class="max-w-3xl mx-auto px-6 text-center relative">
		<h2 class="text-3xl md:text-5xl font-black text-white mb-6">
			Ready to stop being your own secretary?
		</h2>
		<p class="text-gray-400 text-lg mb-10 max-w-xl mx-auto leading-relaxed">
			30 minutes. We'll learn your workflow, show you exactly what your AI Chief of Staff would handle,
			and you decide if it makes sense. No slides. No pressure. Just a real conversation.
		</p>
		<a
			href="https://calendly.com"
			target="_blank"
			rel="noopener noreferrer"
			class="inline-block bg-[#f97316] hover:bg-[#fb923c] text-white px-10 py-4 rounded-lg font-bold text-lg transition-colors shadow-lg shadow-[#f97316]/25"
		>
			Book Your Discovery Call
		</a>
		<p class="text-gray-600 text-sm mt-6">Taking on a limited number of new clients right now.</p>
	</div>
</section>

<!-- Footer -->
<footer class="bg-[#0f1117] border-t border-white/5 py-12">
	<div class="max-w-6xl mx-auto px-6">
		<div class="flex flex-col md:flex-row items-center justify-between gap-4">
			<div class="text-white font-bold text-lg">
				Open<span class="text-[#f97316]">Claw</span>
			</div>
			<p class="text-gray-600 text-sm">
				We sell architecture and leverage. Not compute.
			</p>
			<p class="text-gray-600 text-sm">
				&copy; {new Date().getFullYear()} OpenClaw. All rights reserved.
			</p>
		</div>
	</div>
</footer>
