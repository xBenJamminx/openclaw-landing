<script lang="ts">
	import '../app.css';
	let { children } = $props();
</script>

<svelte:head>
	<link rel="preconnect" href="https://fonts.googleapis.com" />
	<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="anonymous" />
	<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800;900&display=swap" rel="stylesheet" />
	<title>OpenClaw — Your AI Chief of Staff</title>
	<meta name="description" content="We build private AI systems that actually run your operations. Inbox triaged. Calendar optimized. Follow-ups tracked. Running 24/7 on your hardware." />
</svelte:head>

{@render children()}
