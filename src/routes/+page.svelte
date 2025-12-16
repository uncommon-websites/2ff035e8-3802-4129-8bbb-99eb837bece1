<script lang="ts">
	// No script needed for static recreation
</script>

<svelte:head>
	<title>Amber Minefee — Product Designer</title>
	<meta name="description" content="Product designer transforming complex systems into empathetic, data-informed experiences. Specializing in healthcare and education UX with research rigor." />
</svelte:head>

<div class="min-h-screen bg-white text-black font-sans px-6 py-8 md:px-10 md:py-10 selection:bg-gray-200">
	<!-- Header -->
	<header class="grid grid-cols-2 md:grid-cols-12 gap-y-4 text-[15px] leading-tight mb-32 md:mb-48 font-normal">
		<div class="col-span-1 md:col-span-3">
			Amber Minefee
		</div>
		
		<div class="col-span-1 md:col-span-2 md:col-start-4">
			<a href="#" class="hover:opacity-60 transition-opacity">Work</a>
		</div>
		
		<div class="col-span-1 md:col-span-2 md:col-start-6">
			<a href="#" class="hover:opacity-60 transition-opacity">About</a>
		</div>
		
		<div class="col-span-1 md:col-span-2 md:col-start-10 text-right md:text-left">
			<a href="#" class="hover:opacity-60 transition-opacity">Resume</a>
		</div>
		
		<div class="col-span-1 md:col-span-1 md:col-start-12 text-right">
			<a href="#" class="hover:opacity-60 transition-opacity">Contact</a>
		</div>
	</header>

	<!-- Hero -->
	<section class="grid grid-cols-1 md:grid-cols-12 mb-32 md:mb-48">
		<div class="col-span-1 md:col-span-9 md:col-start-4 text-[28px] md:text-[32px] leading-[1.15] tracking-tight font-normal">
			<p>
				I'm a product designer who transforms complex systems into empathetic, data-informed experiences. With a background in healthcare and biology, I bring research rigor and human-centered thinking to every project—creating products that drive positive change and empower the underrepresented.
			</p>
		</div>
	</section>

	<!-- Projects -->
	<section class="flex flex-col gap-24 md:gap-32 mb-32">
		<!-- Project 1 -->
		<article class="grid grid-cols-1 md:grid-cols-12">
			<div class="col-span-1 md:col-span-9 md:col-start-4 grid grid-cols-1 md:grid-cols-12 mb-3 text-[15px] gap-y-1 items-baseline">
				<div class="col-span-1 md:col-span-4 font-normal">
					Longitudinal Care
				</div>
				<div class="col-span-1 md:col-span-8 text-gray-400 font-normal">
					Healthcare UX and product design translating complex medical systems into intuitive patient experiences.
				</div>
			</div>
			<div class="col-span-1 md:col-span-9 md:col-start-4 w-full aspect-[16/10] bg-gray-100 overflow-hidden relative group cursor-pointer">
				<img 
					src="https://images.unsplash.com/photo-1576091160399-112ba8d25d1d?q=80&w=2500&auto=format&fit=crop" 
					alt="Longitudinal Care Healthcare Interface" 
					class="w-full h-full object-cover brightness-95 transition-transform duration-700 group-hover:scale-105"
				/>
				<div class="absolute inset-0 flex items-center justify-center pointer-events-none">
					<div class="bg-white/95 px-8 py-6 rounded-sm shadow-lg">
						<span class="text-gray-900 font-medium text-4xl md:text-6xl tracking-tight">Healthcare</span>
					</div>
				</div>
			</div>
		</article>

		<!-- Project 2 -->
		<article class="grid grid-cols-1 md:grid-cols-12">
			<div class="col-span-1 md:col-span-9 md:col-start-4 grid grid-cols-1 md:grid-cols-12 mb-3 text-[15px] gap-y-1 items-baseline">
				<div class="col-span-1 md:col-span-4 font-normal">
					Green St K-12
				</div>
				<div class="col-span-1 md:col-span-8 text-gray-400 font-normal">
					Education platform design and UX research empowering teachers and students through thoughtful interaction.
				</div>
			</div>
			<div class="col-span-1 md:col-span-9 md:col-start-4 w-full aspect-[16/10] bg-primary-50 overflow-hidden relative group cursor-pointer">
				<img 
					src="https://images.unsplash.com/photo-1503676260728-1c00da094a0b?q=80&w=2500&auto=format&fit=crop" 
					alt="Green St K-12 Education Platform" 
					class="w-full h-full object-cover opacity-80 mix-blend-multiply transition-transform duration-700 group-hover:scale-105"
				/>
				<div class="absolute inset-0 flex items-center justify-center pointer-events-none">
					<div class="bg-primary-500/90 px-8 py-6 rounded-sm shadow-lg">
						<span class="text-white font-medium text-4xl md:text-6xl tracking-tight">Education</span>
					</div>
				</div>
			</div>
		</article>

		<!-- Project 3 -->
		<article class="grid grid-cols-1 md:grid-cols-12">
			<div class="col-span-1 md:col-span-9 md:col-start-4 grid grid-cols-1 md:grid-cols-12 mb-3 text-[15px] gap-y-1 items-baseline">
				<div class="col-span-1 md:col-span-4 font-normal">
					Green Thumb
				</div>
				<div class="col-span-1 md:col-span-8 text-gray-400 font-normal">
					Consumer product design and visual design helping people cultivate their connection with plants.
				</div>
			</div>
			<div class="col-span-1 md:col-span-9 md:col-start-4 w-full aspect-[16/10] bg-[#1a4d2e] overflow-hidden relative group cursor-pointer">
				<img 
					src="https://images.unsplash.com/photo-1466781783364-36c955e42a7f?q=80&w=2500&auto=format&fit=crop" 
					alt="Green Thumb Plant Care App" 
					class="w-full h-full object-cover opacity-75 transition-transform duration-700 group-hover:scale-105"
				/>
				<div class="absolute inset-0 flex items-center justify-center pointer-events-none">
					<div class="flex items-center gap-3">
						<svg class="w-12 h-12 md:w-16 md:h-16 text-[#86efac]" viewBox="0 0 24 24" fill="currentColor">
							<path d="M12 2C8.13 2 5 5.13 5 9c0 5.25 7 13 7 13s7-7.75 7-13c0-3.87-3.13-7-7-7zm0 9.5c-1.38 0-2.5-1.12-2.5-2.5s1.12-2.5 2.5-2.5 2.5 1.12 2.5 2.5-1.12 2.5-2.5 2.5z"/>
						</svg>
						<span class="text-[#86efac] font-medium text-5xl md:text-7xl tracking-tight">Green Thumb</span>
					</div>
				</div>
			</div>
		</article>

		<div class="grid grid-cols-1 md:grid-cols-12 text-[15px]">
			<div class="col-span-1 md:col-span-2 md:col-start-4">
				<a href="#" class="hover:opacity-60 transition-opacity">View all work</a>
			</div>
		</div>
	</section>

	<!-- Footer -->
	<footer class="border-t border-gray-200 pt-6 md:pt-8 text-[13px] leading-relaxed text-gray-400 font-normal">
		<div class="grid grid-cols-1 md:grid-cols-12 gap-y-8">
			<div class="col-span-1 md:col-span-3">
				&copy; Amber Minefee
			</div>

			<div class="col-span-1 md:col-span-2 md:col-start-4 flex flex-col gap-0.5">
				<a href="#" class="hover:text-black transition-colors">LinkedIn</a>
				<a href="#" class="hover:text-black transition-colors">Dribbble</a>
				<a href="#" class="hover:text-black transition-colors">Email</a>
			</div>

			<div class="col-span-1 md:col-span-3 md:col-start-6">
				<p>Los Angeles, CA</p>
				<p>Available for freelance</p>
				<p>and contract work</p>
			</div>
		</div>

		<div class="grid grid-cols-1 md:grid-cols-12 mt-12 md:mt-24">
			<div class="col-span-1 md:col-span-6 md:col-start-4 text-gray-400">
				<p>
					I'm committed to creating inclusive, accessible design that empowers underrepresented communities. My work centers on empathy, research rigor, and human-centered thinking—transforming complex systems into experiences that help people spend more time on what matters most.
				</p>
			</div>
		</div>
	</footer>
</div>

