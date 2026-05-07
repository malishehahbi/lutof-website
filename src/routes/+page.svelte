<script lang="ts">
	import favicon from '$lib/assets/favicon.svg';
</script>

<svelte:head>
	<title>Lutof - See Your LUTs Instantly</title>
	<meta name="description" content="The fastest way to preview, compare, and manage your color grading library." />
</svelte:head>

<a href="#main-content" class="sr-only focus:not-sr-only focus:absolute focus:top-4 focus:left-4 focus:z-50 focus:px-4 focus:py-2 focus:bg-primary focus:text-primary-foreground focus:rounded-md focus:outline-none">
	Skip to main content
</a>

<div class="min-h-screen bg-background text-foreground dark" dir="ltr">
	<!-- Hero Section -->
	<section class="px-4 py-20 sm:px-6 sm:py-28 md:py-32">
		<div class="container mx-auto max-w-4xl text-center">
			<h1 class="animate-fade-in-up font-sans text-5xl sm:text-6xl md:text-7xl font-bold tracking-tightest text-balance leading-[0.95]">
				See your LUTs. <span class="text-primary">Instantly.</span>
			</h1>
			<p class="animate-fade-in-up animation-delay-100 mx-auto mt-6 max-w-xl text-lg text-muted-foreground leading-relaxed-custom">
				The fastest way to preview and compare your color grading library.
			</p>
			<div class="animate-fade-in-up animation-delay-200 mt-10 flex flex-col items-center gap-4">
				<a
					href="#download"
					class="inline-flex h-12 min-w-[200px] items-center justify-center rounded-lg bg-primary px-8 text-sm font-semibold text-primary-foreground transition-all duration-200 ease-out hover:scale-[1.02] hover:shadow-lg hover:shadow-primary/20 focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 focus-visible:ring-offset-background active:scale-[0.98]"
				>
					Download for Windows
				</a>
				<span class="text-sm text-muted-foreground">Mac version coming soon</span>
			</div>
		</div>
	</section>

	<!-- Problem vs Solution -->
	<section class="px-4 py-16 sm:px-6 md:py-20">
		<div class="container mx-auto max-w-3xl">
			<div class="grid sm:grid-cols-2 gap-8">
				<div class="space-y-3 animate-fade-in-up animation-delay-300">
					<h2 class="text-xl font-semibold text-destructive">The Old Way</h2>
					<p class="text-muted-foreground leading-relaxed-custom">
						Click through LUTs one by one in your editor. Wait for each to load. Waste hours.
					</p>
				</div>
				<div class="space-y-3 animate-fade-in-up animation-delay-400">
					<h2 class="text-xl font-semibold text-primary">The Lutof Way</h2>
					<p class="text-muted-foreground leading-relaxed-custom">
						Drop a folder of LUTs. See them all instantly. Find your look in seconds.
					</p>
				</div>
			</div>
		</div>
	</section>

	<!-- Features -->
	<section class="px-4 py-16 sm:px-6 md:py-20" aria-label="Features">
		<div class="container mx-auto max-w-4xl space-y-16">
			<h2 class="text-3xl font-bold text-center tracking-tightest">Core Features</h2>

			<!-- Feature 1 -->
			<div class="grid sm:grid-cols-2 gap-8 items-center">
				<div class="space-y-3">
					<h3 class="text-2xl font-semibold tracking-tightest">Instant Grid</h3>
					<p class="text-muted-foreground leading-relaxed-custom">
						Drop your photo and a folder of LUTs. See every LUT applied instantly in a scrollable grid.
					</p>
				</div>
				<div class="aspect-video rounded-lg border border-border/30 bg-muted/10 flex items-center justify-center transition-all duration-300 hover:border-primary/30" role="img" aria-label="Instant grid feature demonstration">
					<p class="text-sm text-muted-foreground/60">Insert masonry grid demo GIF</p>
				</div>
			</div>

			<!-- Feature 2 -->
			<div class="grid sm:grid-cols-2 gap-8 items-center">
				<div class="order-2 sm:order-1 space-y-3">
					<h3 class="text-2xl font-semibold tracking-tightest">Compare Tools</h3>
					<p class="text-muted-foreground leading-relaxed-custom">
						Split-screen sliders and hover-to-compare. Find the perfect look without switching apps.
					</p>
				</div>
				<div class="order-1 sm:order-2 aspect-video rounded-lg border border-border/30 bg-muted/10 flex items-center justify-center transition-all duration-300 hover:border-primary/30" role="img" aria-label="Compare tools feature demonstration">
					<p class="text-sm text-muted-foreground/60">Insert split-slider demo GIF</p>
				</div>
			</div>

			<!-- Feature 3 -->
			<div class="grid sm:grid-cols-2 gap-8 items-center">
				<div class="space-y-3">
					<h3 class="text-2xl font-semibold tracking-tightest">Library Management</h3>
					<p class="text-muted-foreground leading-relaxed-custom">
						Drag-select multiple LUTs, bulk-delete the ones you don't need. Organize in seconds.
					</p>
				</div>
				<div class="aspect-video rounded-lg border border-border/30 bg-muted/10 flex items-center justify-center transition-all duration-300 hover:border-primary/30" role="img" aria-label="Library management feature demonstration">
					<p class="text-sm text-muted-foreground/60">Insert bulk management demo GIF</p>
				</div>
			</div>
		</div>
	</section>

	<!-- CTA -->
	<section id="download" class="px-4 py-16 sm:px-6 md:py-20">
		<div class="container mx-auto max-w-xl text-center">
			<h2 class="text-3xl font-bold tracking-tightest">Ready to speed up your workflow?</h2>
			<p class="mt-4 text-muted-foreground leading-relaxed-custom">
				Download Lutof for Windows.
			</p>
			<div class="mt-8">
				<a
					href="#"
					class="inline-flex h-12 min-w-[200px] items-center justify-center rounded-lg bg-primary px-8 text-sm font-semibold text-primary-foreground transition-all duration-200 ease-out hover:scale-[1.02] hover:shadow-lg hover:shadow-primary/20 focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 focus-visible:ring-offset-background active:scale-[0.98]"
				>
					Download for Windows
				</a>
			</div>
		</div>
	</section>

	<!-- Footer -->
	<footer class="border-t border-border/30 px-4 py-8 sm:px-6" role="contentinfo">
		<div class="container mx-auto flex flex-col sm:flex-row items-center justify-between gap-4">
			<div class="flex items-center gap-2">
				<img src={favicon} alt="Lutof" class="h-6 w-6" />
				<span class="font-semibold">Lutof</span>
			</div>
			<p class="text-sm text-muted-foreground">
				&copy; 2025 Lutof
			</p>
			<nav class="flex items-center gap-4" aria-label="Social links">
				<a 
					href="https://twitter.com" 
					target="_blank" 
					rel="noopener noreferrer" 
					class="flex h-10 w-10 items-center justify-center rounded-md text-muted-foreground transition-all duration-200 hover:text-foreground hover:bg-muted/50 focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 focus-visible:ring-offset-background" 
					aria-label="Lutof on Twitter (opens in new tab)"
				>
					<svg class="w-5 h-5" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2"><path stroke-linecap="round" stroke-linejoin="round" d="M22 4s-.7 2.1-2 3.4c1.6 10-9.4 17.3-18 11.6 2.2.1 4.4-.6 6-2C3 15.5.5 9.6 3 5c2.2 2.6 5.6 4.1 9 4-.9-4.2 4-6.6 7-3.8 1.1 0 3-1.2 3-1.2z"/></svg>
				</a>
				<a 
					href="mailto:hello@lutof.com" 
					class="flex h-10 w-10 items-center justify-center rounded-md text-muted-foreground transition-all duration-200 hover:text-foreground hover:bg-muted/50 focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 focus-visible:ring-offset-background" 
					aria-label="Contact Lutof via email"
				>
					<svg class="w-5 h-5" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2"><rect x="2" y="4" width="20" height="16" rx="2"/><path d="m22 7-8.97 5.7a1.94 1.94 0 01-2.06 0L2 7"/></svg>
				</a>
			</nav>
		</div>
	</footer>
</div>