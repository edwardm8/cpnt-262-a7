<script>
	import '../../app.postcss'
	import { AppShell,LightSwitch, AppBar } from '@skeletonlabs/skeleton'
</script>

<AppShell>
	<svelte:fragment slot="header">
		<AppBar>
			<svelte:fragment slot="lead">
				<strong class="text-xl uppercase">Logo</strong>
			</svelte:fragment>
			<svelte:fragment slot="trail">
				<a class="btn variant-filled" href="/">Home</a>
				<a class="btn variant-filled" href="/about">About</a>
				<a class="btn variant-filled" href="../products">Products</a>
			</svelte:fragment>
			<LightSwitch />
		</AppBar>
	</svelte:fragment>
	<slot />
	<svelte:fragment slot="footer"><AppBar>Footer</AppBar></svelte:fragment>
</AppShell>


