<script lang="ts">
	import favicon from '$lib/assets/favicon.svg';
</script>

<svelte:head>
	<title>Lutof — See Your LUTs Instantly</title>
	<meta name="description" content="The fastest way to preview, compare, and manage your color grading library." />
</svelte:head>

<a href="#main-content" class="sr-only focus:not-sr-only focus:absolute focus:top-4 focus:left-4 focus:z-50 focus:px-4 focus:py-2 focus:bg-primary focus:text-primary-foreground focus:rounded-lg focus:outline-none focus:ring-2 focus:ring-ring focus:ring-offset-2 focus:ring-offset-background">
	Skip to main content
</a>

<!-- Hero -->
<section class="px-4 pt-24 pb-20 sm:px-6 sm:pt-32 sm:pb-28 md:pt-40 md:pb-32">
	<div class="container mx-auto max-w-3xl text-center">
		<h1 class="typo-display text-balance">
			See your LUTs. <strong class="font-black">Instantly.</strong>
		</h1>
		<p class="typo-body mx-auto mt-6 max-w-prose text-muted-foreground text-balance">
			The fastest way to preview, compare, and manage your color grading library.
		</p>
		<div class="mt-10 flex flex-col items-center gap-4">
			<a
				href="#download"
				class="typo-label inline-flex h-12 min-w-[200px] items-center justify-center rounded-lg bg-primary px-8 text-primary-foreground transition-all duration-200 ease-out hover:scale-[1.02] hover:shadow-[0_0_20px] hover:shadow-primary/20 focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 focus-visible:ring-offset-background active:scale-[0.98]"
			>
				Download for Windows
			</a>
			<span class="typo-body text-sm text-muted-foreground">Mac version coming soon</span>
		</div>
	</div>
</section>

<!-- Problem / Solution -->
<section class="border-t border-border px-4 py-16 sm:px-6 md:py-20">
	<div class="container mx-auto max-w-3xl">
		<div class="grid sm:grid-cols-2 gap-12 sm:gap-16">
			<div class="space-y-3">
				<h2 class="typo-title text-destructive">The Old Way</h2>
				<p class="typo-body text-muted-foreground max-w-prose">
					Click through LUTs one by one in your editor. Wait for each to load. Waste hours finding the right look.
				</p>
			</div>
			<div class="space-y-3">
				<h2 class="typo-title text-primary">The Lutof Way</h2>
				<p class="typo-body text-muted-foreground max-w-prose">
					Drop a folder of LUTs. See them all applied instantly on your reference image. Find your look in seconds.
				</p>
			</div>
		</div>
	</div>
</section>

<!-- Features -->
<section class="px-4 py-20 sm:px-6 md:py-28" aria-label="Features">
	<div class="container mx-auto max-w-5xl">
		<h2 class="typo-headline text-center">Core Features</h2>

		<div class="mt-16 space-y-24">
			<!-- Instant Grid -->
			<div class="grid sm:grid-cols-2 gap-10 items-center">
				<div class="space-y-4">
					<h3 class="typo-title">Instant Grid</h3>
					<p class="typo-body text-muted-foreground max-w-prose">
						Drop your photo and a folder of LUTs. See every look applied instantly in a scrollable grid. No waiting, no switching contexts.
					</p>
				</div>
				<div class="aspect-video rounded-lg border border-border/30 bg-muted/10 flex items-center justify-center transition-all duration-300 hover:border-primary/30" role="img" aria-label="Grid of LUT previews shown side by side">
					<span class="typo-label text-muted-foreground/60">Grid preview</span>
				</div>
			</div>

			<!-- Compare Tools -->
			<div class="grid sm:grid-cols-2 gap-10 items-center">
				<div class="order-2 sm:order-1 aspect-video rounded-lg border border-border/30 bg-muted/10 flex items-center justify-center transition-all duration-300 hover:border-primary/30" role="img" aria-label="Split-screen comparison of two LUTs">
					<span class="typo-label text-muted-foreground/60">Side-by-side comparison</span>
				</div>
				<div class="order-1 sm:order-2 space-y-4">
					<h3 class="typo-title">Compare Tools</h3>
					<p class="typo-body text-muted-foreground max-w-prose">
						Split-screen sliders, hover-to-peek, and side-by-side views. Find the perfect grade without switching apps.
					</p>
				</div>
			</div>

			<!-- Library Management -->
			<div class="grid sm:grid-cols-2 gap-10 items-center">
				<div class="space-y-4">
					<h3 class="typo-title">Library Management</h3>
					<p class="typo-body text-muted-foreground max-w-prose">
						Drag-select multiple LUTs, bulk-delete what you don't need, rename in place. Organize your library in seconds, not hours.
					</p>
				</div>
				<div class="aspect-video rounded-lg border border-border/30 bg-muted/10 flex items-center justify-center transition-all duration-300 hover:border-primary/30" role="img" aria-label="Library management interface showing selected LUTs">
					<span class="typo-label text-muted-foreground/60">Bulk management</span>
				</div>
			</div>
		</div>
	</div>
</section>

<!-- CTA -->
<section id="download" class="border-t border-border px-4 py-20 sm:px-6 md:py-28">
	<div class="container mx-auto max-w-xl text-center">
		<h2 class="typo-headline">Ready to speed up your workflow?</h2>
		<p class="typo-body mt-4 text-muted-foreground text-balance">
			Download Lutof for Windows and start previewing LUTs the fast way.
		</p>
		<div class="mt-8">
			<!-- svelte-ignore a11y_invalid_attribute -->
			<a
				href="#"
				class="typo-label inline-flex h-12 min-w-[200px] items-center justify-center rounded-lg bg-primary px-8 text-primary-foreground transition-all duration-200 ease-out hover:scale-[1.02] hover:shadow-[0_0_20px] hover:shadow-primary/20 focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 focus-visible:ring-offset-background active:scale-[0.98]"
			>
				Download for Windows
			</a>
		</div>
	</div>
</section>

<!-- Footer -->
<footer class="border-t border-border px-4 py-8 sm:px-6">
	<div class="container mx-auto flex flex-col sm:flex-row items-center justify-between gap-6">
		<div class="flex items-center gap-2">
			<img src={favicon} alt="Lutof" class="h-5 w-5" />
			<span class="font-semibold text-base">Lutof</span>
		</div>
		<nav class="flex items-center gap-6" aria-label="Social links">
			<a
				href="https://twitter.com"
				target="_blank"
				rel="noopener noreferrer"
				class="text-sm text-muted-foreground transition-all duration-200 hover:text-foreground hover:bg-muted/50 px-2 py-1 rounded focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 focus-visible:ring-offset-background"
				aria-label="Lutof on Twitter (opens in new tab)"
			>
				Twitter
			</a>
			<a
				href="mailto:hello@lutof.com"
				class="text-sm text-muted-foreground transition-all duration-200 hover:text-foreground hover:bg-muted/50 px-2 py-1 rounded focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 focus-visible:ring-offset-background"
				aria-label="Contact Lutof via email"
			>
				Email
			</a>
		</nav>
		<p class="text-sm text-muted-foreground">&copy; 2025 Lutof</p>
	</div>
</footer>
