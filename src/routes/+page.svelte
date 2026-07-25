<script>
	const specs = [
		{
			label: 'GPU',
			value: 'Nvidia GeForce RTX 5070'
		},
		{
			label: 'CPU',
			value: 'Ryzen 5 7600 6-Core'
		},
		{
			label: 'Motherboard',
			value: 'Gigabyte B650 EAGLE AX'
		},
		{
			label: 'Case',
			value: 'NZXT H9 Flow'
		},
		{
			label: 'RAM 2x',
			value: '32GB DDR5 4800MMT/s'
		},
		{
			label: 'Storage 2x',
			value: 'Samsung SSD 990 Pro 1TB'
		},
		{
			label: 'Power Supply',
			value: '750W Gold Certified (Not sure currently)'
		},
		{
			label: 'Mouse',
			value: 'Logitech Super Light PRO (White)'
		},
		{
			label: 'Keyboard',
			value: 'Selfbuild Mechanical Keyboard (Blue and Tiget Switches)'
		},
		{
			label: 'Monitor 1x',
			value: 'HP X24c'
		},
		{
			label: 'Monitor 2x',
			value: 'R27qe'
		},
		{
			label: 'Monitor 3x - Currently Broken',
			value: 'R27qe'
		},
		{
			label: "Laptop",
			value: "HP OmniBook 6 15"
		}
	];

	const lastEdited = '7/25/2026';
</script>

<main class="flex min-h-screen items-center justify-center bg-zinc-950 px-4 text-zinc-100">
	<div class="w-full max-w-md">
		<h1 class="mb-8 text-center text-3xl font-semibold">My PC specs</h1>

		<div class="space-y-3">
			{#each specs as spec}
				<div
					class="block rounded-xl border border-zinc-800 bg-zinc-900 px-4 py-3 transition hover:border-zinc-700 hover:bg-zinc-800"
				>
					<div class="text-xs tracking-wide text-zinc-400 uppercase">
						{spec.label}
					</div>
					<div class="text-lg font-medium">
						{spec.value}
					</div>
				</div>
			{/each}
		</div>

		<div class="mt-8 text-center text-xs text-zinc-500">
			Last edited: {lastEdited}
		</div>
	</div>
</main>
