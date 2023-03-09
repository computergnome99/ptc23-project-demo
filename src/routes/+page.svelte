<svelte:head>
	<title>Home</title>
	<meta
		name="description"
		content="My name is Calvin Bonner, I am a Front-End and Service-Layer developer from Grand Rapids MI
			with experience in numerous technical fields and across multiple tech-stacks."
	/>
</svelte:head>

<section class="bg-white">
	<div class="relative isolate overflow-hidden bg-gradient-to-b from-indigo-100/20">
		<div
			class="mx-auto max-w-7xl pt-10 pb-24 sm:pb-28 lg:grid lg:grid-cols-2 lg:gap-x-8 lg:py-40 lg:px-8"
		>
			<div class="px-6 lg:px-0 lg:pt-4">
				<div class="mx-auto max-w-2xl">
					<div class="max-w-lg">
						<h1 class="mt-10 text-4xl font-bold tracking-tight text-gray-900 sm:text-6xl">
							Hi, my name is Calvin Bonner
						</h1>
						<p class="mt-6 text-lg leading-8 text-gray-600">
							I believe that products are built for users - not just to solve abstract technical
							problems. The most technically innovative code is worthless if the end-user experience
							is subpar.
						</p>
						<div class="mt-10 flex items-center flex-wrap gap-6">
							<a
								href="/about#code"
								class="max-[410px]:flex-grow max-[410px]:text-center rounded-md bg-indigo-600 px-3.5 py-2.5 text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600"
							>
								My approach to code
								<span class="sr-only"> - opens in a new tab.</span>
							</a>
							<a
								href="/about"
								class="max-[410px]:flex-grow max-[410px]:text-center rounded-md px-3.5 py-2.5 text-sm font-semibold leading-6 text-gray-900"
							>
								More about me <span aria-hidden="true">→</span>
							</a>
						</div>
					</div>
				</div>
			</div>
			<div class="mt-20 sm:mt-24 md:mx-auto md:max-w-2xl lg:mx-0 lg:mt-0 lg:w-screen">
				<div
					class="absolute inset-y-0 right-1/2 -z-10 -mr-10 w-[200%] skew-x-[-30deg] bg-white shadow-xl shadow-indigo-600/10 ring-1 ring-indigo-50 md:-mr-20 lg:-mr-36"
					aria-hidden="true"
				/>
				<img class="shadow-lg md:rounded-3xl overflow-hidden" src="/hero.webp" alt="My face" />
			</div>
		</div>
		<div class="absolute inset-x-0 bottom-0 -z-10 h-24 bg-gradient-to-t from-white sm:h-32" />
	</div>
</section>

<section class="bg-white py-24 sm:py-28">
	<div class="mx-auto max-w-7xl px-6 lg:px-8">
		<div class="mx-auto grid max-w-2xl grid-cols-1 lg:mx-0 lg:max-w-none lg:grid-cols-2">
			<div class="flex flex-col pb-10 sm:pb-16 lg:pb-0 lg:pr-8 xl:pr-20">
				<img class="h-12 self-start" src="/gc-logo.svg" alt="" />
				<figure class="mt-10 flex flex-auto flex-col justify-between">
					<blockquote class="text-lg leading-8 text-gray-900">
						<p>
							“He not only reduced loading time by implementing the right technology but also
							ensured that [our website] is attractive and easy-to-use. [...] He understands the
							needs and budgetary constraints of a small business.”
						</p>
					</blockquote>
					<figcaption class="mt-10 flex items-center gap-x-6">
						<img
							class="h-14 w-14 rounded-full bg-gray-50"
							src="/steve-mete.webp"
							alt="Steven Mete"
						/>
						<div class="text-base">
							<div class="font-semibold text-gray-900">Steven Mete</div>
							<div class="mt-1 text-gray-500">Sales Manager at Gage Crib Worldwide Inc.</div>
						</div>
					</figcaption>
				</figure>
			</div>
			<div
				class="flex flex-col border-t border-gray-900/10 pt-10 sm:pt-16 lg:border-t-0 lg:border-l lg:pt-0 lg:pl-8 xl:pl-20"
			>
				<img class="h-12 w-3/6 self-start" src="/tlc-logo.svg" alt="" />
				<figure class="mt-10 flex flex-auto flex-col justify-between">
					<blockquote class="text-lg leading-8 text-gray-900">
						<p>
							“It's not easy to translate what someone desires into a quality product but Calvin's
							communication and flexibility made it a great process to reach the finished product.”
						</p>
					</blockquote>
					<figcaption class="mt-10 flex items-center gap-x-6">
						<img
							class="h-14 w-14 rounded-full bg-gray-50"
							src="/jordan-koller.webp"
							alt="Jordan Koller"
						/>
						<div class="text-base">
							<div class="font-semibold text-gray-900">Jordan Koller</div>
							<div class="mt-1 text-gray-500">Pastor of Worship Culture at The Local Church GR</div>
						</div>
					</figcaption>
				</figure>
			</div>
		</div>
	</div>
</section>

<section class="mx-auto max-w-7xl py-24 sm:px-6 sm:py-32 lg:px-8">
	<div
		class="relative isolate overflow-hidden bg-gradient-to-b from-indigo-100 to-indigo-50 px-6 py-24 text-center shadow-2xl sm:rounded-3xl sm:px-16"
	>
		<h2 class="text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">
			Ready to take the next step?<br />Let's develop something great together.
		</h2>
		<p class="mx-auto mt-6 max-w-xl text-lg leading-8 text-gray-600">
			I believe in doing all things to the best of my ability. I build products to be robust,
			accessible, and as simple as possible. Contact me today to get started on the next step of
			your product's journey.
		</p>
		<div class="mt-10 flex items-center justify-center gap-x-6">
			<a
				href="/contact"
				class="rounded-md bg-indigo-600 px-3.5 py-2.5 text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600"
			>
				Contact me
			</a>
			<a href="/about" class="text-sm font-semibold leading-6 text-gray-900">
				More about me <span aria-hidden="true">→</span>
			</a>
		</div>
	</div>
</section>
