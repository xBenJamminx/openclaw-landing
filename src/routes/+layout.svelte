<script lang="ts">
	import '../app.css';
	let { children } = $props();
</script>

<svelte:head>
	<link rel="preconnect" href="https://fonts.googleapis.com" />
	<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="anonymous" />
	<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800;900&display=swap" rel="stylesheet" />
	<title>OpenClaw — Private AI Infrastructure for Operators</title>
	<meta name="description" content="Your AI Chief of Staff — configured, secured, and maintained. Premium AI infrastructure for founders, executives, and high-performing households." />
</svelte:head>

{@render children()}
