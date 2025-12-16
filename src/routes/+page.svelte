<script lang="ts">
	import { onMount } from 'svelte';
	
	let currentTime = $state('');
	let isAvailable = $state(true);
	
	onMount(() => {
		const updateTime = () => {
			const now = new Date();
			const hours = now.getHours().toString().padStart(2, '0');
			const minutes = now.getMinutes().toString().padStart(2, '0');
			const seconds = now.getSeconds().toString().padStart(2, '0');
			currentTime = `${hours}:${minutes}:${seconds}`;
		};
		
		updateTime();
		const interval = setInterval(updateTime, 1000);
		
		return () => clearInterval(interval);
	});
</script>

<svelte:head>
	<title>Amber Minefee — Product Designer</title>
	<meta name="description" content="Product designer transforming complex systems into empathetic, data-informed experiences. Specializing in healthcare and education UX with research rigor." />
</svelte:head>

<div class="min-h-screen bg-white text-black font-sans selection:bg-gray-200">
	<!-- Corner markers -->
	<div class="fixed top-6 left-6 w-6 h-6 border-l-2 border-t-2 border-black pointer-events-none z-50"></div>
	<div class="fixed top-6 right-6 w-6 h-6 border-r-2 border-t-2 border-black pointer-events-none z-50"></div>
	<div class="fixed bottom-6 left-6 w-6 h-6 border-l-2 border-b-2 border-black pointer-events-none z-50"></div>
	<div class="fixed bottom-6 right-6 w-6 h-6 border-r-2 border-b-2 border-black pointer-events-none z-50"></div>

	<div class="px-6 py-8 md:px-10 md:py-10">
		<!-- Header -->
		<header class="grid grid-cols-1 md:grid-cols-12 gap-y-6 mb-32 md:mb-48">
			<!-- Top row: Name and technical details -->
			<div class="col-span-1 md:col-span-12 flex flex-col md:flex-row md:items-center md:justify-between gap-4 pb-6 border-b border-gray-200">
				<div class="flex items-center gap-4">
					<h1 class="text-[15px] font-semibold tracking-tight uppercase">Amber Minefee</h1>
					<span class="hidden md:inline text-[11px] text-gray-400 tracking-wider uppercase">Product Designer</span>
				</div>
				
				<div class="flex items-center gap-6 text-[11px] text-gray-500 font-mono">
					<div class="flex items-center gap-2">
						<span class="w-1.5 h-1.5 rounded-full bg-green-500"></span>
						<span class="uppercase tracking-wider">{currentTime} PST</span>
					</div>
					<span class="hidden md:inline">(Los Angeles)</span>
					<div class="flex items-center gap-2">
						<span class="w-1.5 h-1.5 rounded-full bg-green-500"></span>
						<span class="uppercase tracking-wider">Available</span>
					</div>
				</div>
			</div>
			
			<!-- Navigation -->
			<nav class="col-span-1 md:col-span-12 flex flex-wrap gap-x-8 gap-y-3 text-[13px] font-medium">
				<a href="#" class="hover:text-gray-500 transition-colors tracking-wide">Work</a>
				<a href="#" class="hover:text-gray-500 transition-colors tracking-wide">About</a>
				<a href="#" class="hover:text-gray-500 transition-colors tracking-wide">Resume</a>
				<a href="#" class="hover:text-gray-500 transition-colors tracking-wide">Contact</a>
			</nav>
		</header>

		<!-- Hero -->
		<section class="grid grid-cols-1 md:grid-cols-12 mb-32 md:mb-48 relative">
			<div class="col-span-1 md:col-span-1 text-[11px] text-gray-400 font-mono tracking-wider mb-4 md:mb-0">
				001
			</div>
			<div class="col-span-1 md:col-span-10 md:col-start-3">
				<div class="text-[32px] md:text-[48px] lg:text-[56px] leading-[1.1] tracking-tight font-light mb-8">
					<p class="mb-6">
						I'm a product designer who transforms <span class="font-semibold">complex systems</span> into empathetic, data-informed experiences.
					</p>
					<p class="text-[20px] md:text-[24px] text-gray-500 font-normal leading-[1.4]">
						With a background in healthcare and biology, I bring research rigor and human-centered thinking to every project—creating products that drive positive change and empower the underrepresented.
					</p>
				</div>
				
				<div class="flex flex-wrap gap-3 text-[11px] font-mono uppercase tracking-wider mt-12">
					<span class="px-3 py-1.5 border border-gray-300 text-gray-600">Healthcare UX</span>
					<span class="px-3 py-1.5 border border-gray-300 text-gray-600">Education Design</span>
					<span class="px-3 py-1.5 border border-gray-300 text-gray-600">Research</span>
					<span class="px-3 py-1.5 border border-gray-300 text-gray-600">Product Strategy</span>
				</div>
			</div>
		</section>

		<!-- Projects Section Header -->
		<div class="grid grid-cols-1 md:grid-cols-12 mb-16 pb-6 border-b border-gray-200">
			<div class="col-span-1 md:col-span-1 text-[11px] text-gray-400 font-mono tracking-wider">
				002
			</div>
			<div class="col-span-1 md:col-span-11 md:col-start-3">
				<h2 class="text-[24px] md:text-[32px] font-semibold tracking-tight mb-2">Selected work</h2>
				<p class="text-[13px] text-gray-500 tracking-wide">Case studies spanning healthcare, education, and consumer products</p>
			</div>
		</div>

		<!-- Projects -->
		<section class="flex flex-col gap-20 md:gap-24 mb-32">
			<!-- Project 1 -->
			<article class="grid grid-cols-1 md:grid-cols-12 group">
				<div class="col-span-1 md:col-span-1 text-[11px] text-gray-400 font-mono tracking-wider mb-4 md:mb-0">
					01
				</div>
				<div class="col-span-1 md:col-span-11 md:col-start-3">
					<div class="mb-6">
						<h3 class="text-[20px] md:text-[24px] font-semibold tracking-tight mb-2">Longitudinal Care</h3>
						<p class="text-[13px] text-gray-500 leading-relaxed max-w-2xl">
							Healthcare UX and product design translating complex medical systems into intuitive patient experiences.
						</p>
						<div class="flex gap-2 mt-3 text-[10px] font-mono uppercase tracking-wider">
							<span class="text-gray-400">Healthcare</span>
							<span class="text-gray-300">•</span>
							<span class="text-gray-400">UX Research</span>
							<span class="text-gray-300">•</span>
							<span class="text-gray-400">Product Design</span>
						</div>
					</div>
					<div class="w-full aspect-[16/9] bg-gray-100 overflow-hidden relative cursor-pointer border border-gray-200">
						<img 
							src="https://images.unsplash.com/photo-1576091160399-112ba8d25d1d?q=80&w=2500&auto=format&fit=crop" 
							alt="Longitudinal Care Healthcare Interface" 
							class="w-full h-full object-cover brightness-95 transition-all duration-700 group-hover:scale-105 group-hover:brightness-90"
						/>
						<div class="absolute inset-0 bg-black/0 group-hover:bg-black/10 transition-all duration-500"></div>
						<div class="absolute bottom-6 right-6 text-[11px] font-mono text-white/0 group-hover:text-white/80 transition-all duration-500 tracking-wider uppercase">
							View Case Study →
						</div>
					</div>
				</div>
			</article>

			<!-- Project 2 -->
			<article class="grid grid-cols-1 md:grid-cols-12 group">
				<div class="col-span-1 md:col-span-1 text-[11px] text-gray-400 font-mono tracking-wider mb-4 md:mb-0">
					02
				</div>
				<div class="col-span-1 md:col-span-11 md:col-start-3">
					<div class="mb-6">
						<h3 class="text-[20px] md:text-[24px] font-semibold tracking-tight mb-2">Green St K-12</h3>
						<p class="text-[13px] text-gray-500 leading-relaxed max-w-2xl">
							Education platform design and UX research empowering teachers and students through thoughtful interaction.
						</p>
						<div class="flex gap-2 mt-3 text-[10px] font-mono uppercase tracking-wider">
							<span class="text-gray-400">Education</span>
							<span class="text-gray-300">•</span>
							<span class="text-gray-400">Platform Design</span>
							<span class="text-gray-300">•</span>
							<span class="text-gray-400">User Research</span>
						</div>
					</div>
					<div class="w-full aspect-[16/9] bg-primary-50 overflow-hidden relative cursor-pointer border border-gray-200">
						<img 
							src="https://images.unsplash.com/photo-1503676260728-1c00da094a0b?q=80&w=2500&auto=format&fit=crop" 
							alt="Green St K-12 Education Platform" 
							class="w-full h-full object-cover opacity-80 mix-blend-multiply transition-all duration-700 group-hover:scale-105"
						/>
						<div class="absolute inset-0 bg-black/0 group-hover:bg-black/10 transition-all duration-500"></div>
						<div class="absolute bottom-6 right-6 text-[11px] font-mono text-gray-900/0 group-hover:text-gray-900/80 transition-all duration-500 tracking-wider uppercase">
							View Case Study →
						</div>
					</div>
				</div>
			</article>

			<!-- Project 3 -->
			<article class="grid grid-cols-1 md:grid-cols-12 group">
				<div class="col-span-1 md:col-span-1 text-[11px] text-gray-400 font-mono tracking-wider mb-4 md:mb-0">
					03
				</div>
				<div class="col-span-1 md:col-span-11 md:col-start-3">
					<div class="mb-6">
						<h3 class="text-[20px] md:text-[24px] font-semibold tracking-tight mb-2">Green Thumb</h3>
						<p class="text-[13px] text-gray-500 leading-relaxed max-w-2xl">
							Consumer product design and visual design helping people cultivate their connection with plants.
						</p>
						<div class="flex gap-2 mt-3 text-[10px] font-mono uppercase tracking-wider">
							<span class="text-gray-400">Consumer</span>
							<span class="text-gray-300">•</span>
							<span class="text-gray-400">Mobile App</span>
							<span class="text-gray-300">•</span>
							<span class="text-gray-400">Visual Design</span>
						</div>
					</div>
					<div class="w-full aspect-[16/9] bg-[#1a4d2e] overflow-hidden relative cursor-pointer border border-gray-200">
						<img 
							src="https://images.unsplash.com/photo-1466781783364-36c955e42a7f?q=80&w=2500&auto=format&fit=crop" 
							alt="Green Thumb Plant Care App" 
							class="w-full h-full object-cover opacity-75 transition-all duration-700 group-hover:scale-105 group-hover:opacity-85"
						/>
						<div class="absolute inset-0 bg-black/0 group-hover:bg-black/10 transition-all duration-500"></div>
						<div class="absolute bottom-6 right-6 text-[11px] font-mono text-white/0 group-hover:text-white/80 transition-all duration-500 tracking-wider uppercase">
							View Case Study →
						</div>
					</div>
				</div>
			</article>

			<div class="grid grid-cols-1 md:grid-cols-12 mt-8">
				<div class="col-span-1 md:col-span-11 md:col-start-3">
					<a href="#" class="inline-flex items-center gap-2 text-[13px] font-medium hover:text-gray-500 transition-colors tracking-wide group">
						<span>View all work</span>
						<span class="transform group-hover:translate-x-1 transition-transform">→</span>
					</a>
				</div>
			</div>
		</section>

		<!-- Footer -->
		<footer class="border-t border-gray-200 pt-12 md:pt-16 mt-32">
			<!-- Main footer content -->
			<div class="grid grid-cols-1 md:grid-cols-12 gap-y-12 mb-16">
				<div class="col-span-1 md:col-span-1 text-[11px] text-gray-400 font-mono tracking-wider">
					003
				</div>
				
				<div class="col-span-1 md:col-span-5 md:col-start-3">
					<h3 class="text-[20px] font-semibold tracking-tight mb-4">Let's work together</h3>
					<p class="text-[13px] text-gray-500 leading-relaxed mb-6">
						I'm committed to creating inclusive, accessible design that empowers underrepresented communities. My work centers on empathy, research rigor, and human-centered thinking—transforming complex systems into experiences that help people spend more time on what matters most.
					</p>
					<a href="#" class="inline-flex items-center gap-2 text-[13px] font-medium hover:text-gray-500 transition-colors tracking-wide group">
						<span>Get in touch</span>
						<span class="transform group-hover:translate-x-1 transition-transform">→</span>
					</a>
				</div>

				<div class="col-span-1 md:col-span-3 md:col-start-9">
					<div class="mb-8">
						<h4 class="text-[11px] font-mono uppercase tracking-wider text-gray-400 mb-3">Connect</h4>
						<div class="flex flex-col gap-2 text-[13px]">
							<a href="#" class="hover:text-gray-500 transition-colors tracking-wide">LinkedIn</a>
							<a href="#" class="hover:text-gray-500 transition-colors tracking-wide">Dribbble</a>
							<a href="#" class="hover:text-gray-500 transition-colors tracking-wide">Email</a>
						</div>
					</div>
					
					<div>
						<h4 class="text-[11px] font-mono uppercase tracking-wider text-gray-400 mb-3">Location</h4>
						<div class="text-[13px] text-gray-600 leading-relaxed">
							<p>Los Angeles, CA</p>
							<p class="text-gray-400 text-[11px] mt-2 font-mono tracking-wider">34.0522° N, 118.2437° W</p>
						</div>
					</div>
				</div>
			</div>

			<!-- Bottom bar -->
			<div class="border-t border-gray-200 pt-6 pb-8">
				<div class="grid grid-cols-1 md:grid-cols-12 gap-y-4">
					<div class="col-span-1 md:col-span-6 md:col-start-3 text-[11px] text-gray-400 font-mono tracking-wider">
						<div class="flex flex-wrap items-center gap-4">
							<span>&copy; 2025 Amber Minefee</span>
							<span class="hidden md:inline">•</span>
							<div class="flex items-center gap-2">
								<span class="w-1.5 h-1.5 rounded-full bg-green-500"></span>
								<span class="uppercase">Available for freelance and contract work</span>
							</div>
						</div>
					</div>
					
					<div class="col-span-1 md:col-span-3 md:col-start-9 text-[11px] text-gray-400 font-mono tracking-wider md:text-right">
						Designed & developed with care
					</div>
				</div>
			</div>
		</footer>
	</div>
</div>

