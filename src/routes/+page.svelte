<script>
	import { goto } from '$app/navigation';

	let username = $state('');
	let password = $state('');

	//let err = {
	//  username: '',
	//  password: ''
	//};

	
</script>

<div class="flex min-h-screen items-center justify-center bg-[#122C4F]">
	<div class="w-full max-w-md p-6">
		<h1 class="text-center text-2xl font-bold text-gray-100">Login</h1>
		<form class="mt-6">
			<!-- Username -->
			<div class="mt-1">
				<div class="relative">
					<input
						id="username"
						type="text"
						placeholder="Username"
						class="mt-1 w-full rounded-full border bg-gray-100 px-10 py-3 text-gray-700 focus:outline-none focus:ring-2 focus:ring-blue-400"
            bind:value={username}
					/>
				</div>
			</div>

			<!-- Password -->
			<div class="mt-1">
				<div class="relative">
					<input
						id="password"
						type="password"
						placeholder="Password"
						class="mt-1 w-full rounded-full border bg-gray-100 px-10 py-3 text-gray-700 focus:outline-none focus:ring-2 focus:ring-blue-400"
            bind:value={password}
					/>
				</div>
			</div>

			<!-- Sign In Button -->
			<div class="mt-6">
				<button
					type="submit"
					class="w-full rounded-full bg-yellow-500 px-4 py-3 font-semibold text-white hover:bg-yellow-600 focus:outline-none focus:ring-2 focus:ring-yellow-400"
				>
					Sign In
				</button>
			</div>
		</form>

		<!-- Sign Up Link -->
		<p class="mt-4 text-center text-sm text-gray-100">
			Dont have an account?
			<a href="/signup" class="cursor-pointer font-medium text-yellow-500 hover:text-yellow-600">
				Sign Up
			</a>
		</p>
	</div>
</div>
