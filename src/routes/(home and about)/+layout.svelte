<script>
	import '../../app.postcss'
	import { AppShell,LightSwitch, AppBar } from '@skeletonlabs/skeleton'
</script>

<AppShell>
	<svelte:fragment slot="header">
		<AppBar 
			slotTrail="place-content-end"
			background="bg-secondary-50-900-token">
			<svelte:fragment slot="lead">
				<strong class="text-xl uppercase">Logo</strong>
			</svelte:fragment>
			<svelte:fragment slot="trail">
				<a class="btn variant-filled bg-tertiary-50-900-hover-token" href="/">Home</a>
				<a class="btn variant-filled bg-tertiary-50-900-hover-token" href="/about">About</a>
				<a class="btn variant-filled bg-tertiary-50-900-hover-token" href="../products">Products</a>
			</svelte:fragment>
			<LightSwitch />
		</AppBar>
	</svelte:fragment>
	<slot />
	<svelte:fragment slot="footer"><AppBar background="bg-secondary-50-900-token">&copy; Edward Mah 2023</AppBar></svelte:fragment>
</AppShell>


