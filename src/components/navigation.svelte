<script>
	import { page } from '$app/stores';

	/**
	 * @type boolean
	 */
	let menuOpen = false;

	let clientY = 0;
</script>

<svelte:window bind:scrollY={clientY} />

<nav
	class="{clientY != 0 || menuOpen ? 'bg-white/75 backdrop-blur' : 'bg-white/0'} transition-colors"
>
	<div class="mx-auto max-w-7xl px-2 sm:px-6 lg:px-8">
		<div class="relative flex h-16 justify-between">
			<div class="absolute inset-y-0 left-0 flex items-center sm:hidden">
				<button
					type="button"
					class="inline-flex items-center justify-center rounded-md p-2 text-gray-400 hover:bg-gray-100 hover:text-gray-500 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-indigo-500"
					aria-controls="mobile-menu"
					aria-expanded="false"
					on:click={() => (menuOpen = !menuOpen)}
				>
					<span class="sr-only">Open main menu</span>
					<svg
						class="h-6 w-6 {menuOpen ? 'hidden' : 'block'}"
						fill="none"
						viewBox="0 0 24 24"
						stroke-width="1.5"
						stroke="currentColor"
						aria-hidden="true"
					>
						<path
							stroke-linecap="round"
							stroke-linejoin="round"
							d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5"
						/>
					</svg>
					<svg
						class="h-6 w-6 {menuOpen ? 'block' : 'hidden'}"
						fill="none"
						viewBox="0 0 24 24"
						stroke-width="1.5"
						stroke="currentColor"
						aria-hidden="true"
					>
						<path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
					</svg>
				</button>
			</div>
			<div class="flex flex-1 items-center justify-center sm:items-stretch sm:justify-start">
				<div class="flex flex-shrink-0 items-center">
					<img class="block h-8 w-8 rounded-full lg:hidden" src="/profile.jpg" alt="My face" />
					<img class="hidden h-8 w-auto rounded-full lg:block" src="/profile.jpg" alt="My face" />
				</div>
				<div class="hidden sm:ml-6 sm:flex sm:space-x-8">
					<a
						href="/"
						class="inline-flex items-center border-b-2 px-1 pt-1 text-sm font-medium
                            {$page.url.pathname === '/'
							? 'border-indigo-500 text-gray-900'
							: 'border-transparent text-gray-500 hover:border-gray-300 hover:text-gray-700'}"
					>
						Home
					</a>
					<a
						href="/about"
						class="inline-flex items-center border-b-2 px-1 pt-1 text-sm font-medium
                            {$page.url.pathname === '/about'
							? 'border-indigo-500 text-gray-900'
							: 'border-transparent text-gray-500 hover:border-gray-300 hover:text-gray-700'}"
					>
						About
					</a>
					<a
						href="/contact"
						class="inline-flex items-center border-b-2 px-1 pt-1 text-sm font-medium
                            {$page.url.pathname === '/contact'
							? 'border-indigo-500 text-gray-900'
							: 'border-transparent text-gray-500 hover:border-gray-300 hover:text-gray-700'}"
					>
						Contact
					</a>
				</div>
			</div>
		</div>
	</div>

	{#if menuOpen}
		<div class="sm:hidden bg-white" id="mobile-menu">
			<div class="space-y-1 pt-2 pb-4">
				<a
					href="/"
					class="block border-l-4 py-2 pl-3 pr-4 text-base font-medium
                        {$page.url.pathname === '/'
						? 'bg-indigo-50 border-indigo-500 text-indigo-700'
						: 'border-transparent text-gray-500 hover:bg-gray-50 hover:border-gray-300 hover:text-gray-700'}"
					on:click={() => (menuOpen = false)}
				>
					Home
				</a>
				<a
					href="/about"
					class="block border-l-4 py-2 pl-3 pr-4 text-base font-medium
                        {$page.url.pathname === '/about'
						? 'bg-indigo-50 border-indigo-500 text-indigo-700'
						: 'border-transparent text-gray-500 hover:bg-gray-50 hover:border-gray-300 hover:text-gray-700'}"
					on:click={() => (menuOpen = false)}
				>
					About
				</a>
				<a
					href="/contact"
					class="block border-l-4 py-2 pl-3 pr-4 text-base font-medium
                        {$page.url.pathname === '/contact'
						? 'bg-indigo-50 border-indigo-500 text-indigo-700'
						: 'border-transparent text-gray-500 hover:bg-gray-50 hover:border-gray-300 hover:text-gray-700'}"
					on:click={() => (menuOpen = false)}
				>
					Contact
				</a>
			</div>
		</div>
	{/if}
</nav>
