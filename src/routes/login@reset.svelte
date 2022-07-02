<svelte:head>
	<title>Twitter / Login</title>
</svelte:head>

<h1 class="sr-only">Login</h1>

<main class="min-h-screen w-full flex items-center justify-center">
	<div
		class="flex flex-col-reverse | md:gap-10 @xl:min-h-screen xl:(grid grid-cols-12 gap-0) 2xl:max-w-8xl"
	>
		<div class="relative | col-span-6 | 2xl:(rounded-2xl overflow-hidden)">
			<img
				src="https://abs.twimg.com/sticky/illustrations/lohp_en_1302x955.png"
				alt=""
				class="w-full h-full object-cover object-center"
			/>
			<i class="bx bxl-twitter absolute position-center text-white text-[25vw] 2xl:text-18xl" />
		</div>
		<section
			class="max-w-xs w-full py-10 m-auto | col-span-6 flex flex-col gap-9 | sm:max-w-sm md:max-w-lg @lg:py-22 lg:max-w-xl"
		>
			<header>
				<h2 class="sr-only">Login Options</h2>
				<div class="h-22 w-full mb-3 | flex justify-start | lg:hidden">
					<i class="bx bxl-twitter text-[4.125rem] text-sky-500" />
				</div>
				<div class="flex flex-col justify-center gap-8 | text-center lg:text-left">
					<span
						class="text-6xl text-left font-extrabold | sm:(text-6xl text-center) lg:text-left 2xl:text-8xl"
					>
						Happening now
					</span>
					<span class="text-4xl font-bold">Join Twitter today.</span>
				</div>
			</header>
			<div class="flex flex-col gap-4">
				<div class="grid gap-6">
					<button
						class="button button--white | flex items-center justify-center gap-2 | transition duration-250"
					>
						<i class="bx bxl-google text-3xl" />
						<span class="text-lg font-bold font-quick | @xl:text-base  2xl:text-xl">
							Sign up with Google
						</span>
					</button>
					<button
						class="button button--white | flex items-center justify-center gap-2 | transition duration-250"
					>
						<i class="bx bxl-apple text-3xl" />
						<span class="text-xl font-bold | @xl:text-base 2xl:text-2xl"> Sign up with Apple </span>
					</button>
				</div>

				<div class="flex items-center justify-center gap-4" role="separator">
					<div class="w-full h-0.5 | bg-zinc-800 rounded-full" />
					<span class="text-lg font-semibold">or</span>
					<div class="w-full h-0.5 | bg-zinc-800 rounded-full" />
				</div>

				<div>
					<button class="button button--sky | w-full mb-2 | transition duration-250">
						<span class="text-lg font-medium | md:text-lg"> Sign up with phone or email </span>
					</button>
					<span class="w-10/12 mx-auto | block | opacity-90 text-sm text-center">
						By signing up, you agree to the
						<span class="text-sky-500 font-bold">Terms of Service</span> and
						<span class="text-sky-500 font-bold">Privacy Policy</span>, including
						<span class="text-sky-500 font-bold">Cookie Use</span>.
					</span>
				</div>

				<div class="flex flex-col gap-6 mt-3">
					<strong class="text-2xl text-center"> Already have an account? </strong>
					<button class="button button--black | transition duration-250">
						<span class="text-lg text-sky-500 font-medium | md:text-xl @xl:text-base">
							Sign in
						</span>
					</button>
				</div>
			</div>
		</section>
	</div>
</main>

<style>
	.position-center {
		@apply bottom-1/2 right-1/2 transform translate-x-1/2 translate-y-1/2;
	}

	.button {
		@apply h-12 px-6 py-3 rounded-full outline-none @xl:py-2;
	}

	.button--sky {
		@apply bg-sky-500 text-white hover:bg-sky-600 focus:(ring-3 ring-white);
	}

	.button--white {
		@apply bg-white text-zinc-900 hover:bg-zinc-300 focus:(ring-3 ring-sky-400);
	}

	.button--black {
		@apply border-2 border-zinc-300 hover:bg-sky-100 hover:border-transparent focus:(border-transparent ring-3 ring-sky-500);
	}
</style>
