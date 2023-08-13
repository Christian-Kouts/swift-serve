<script>
	import { AppBar, modalStore } from '@skeletonlabs/skeleton';

	function triggerSearch() {
		const modal = {
			type: 'component',
			component: 'modalSearch',
			position: 'item-start'
		};
		modalStore.trigger(modal);
	}
</script>

<AppBar shadow="shadow-lg !bg-transparent">
	<svelte:fragment slot="lead">
		<!-- (case tabs) -->
	</svelte:fragment>
	SwiftServe
	<svelte:fragment slot="trail">
		<!-- <div class="flex justify-end"> -->
		<button type="button" class="btn btn-icon variant-filled shadow-lg" on:click={triggerSearch}
			><svg
				xmlns="http://www.w3.org/2000/svg"
				height="1em"
				viewBox="0 0 512 512"
				style="color: azure;"
				><path
					d="M416 208c0 45.9-14.9 88.3-40 122.7L502.6 457.4c12.5 12.5 12.5 32.8 0 45.3s-32.8 12.5-45.3 0L330.7 376c-34.4 25.2-76.8 40-122.7 40C93.1 416 0 322.9 0 208S93.1 0 208 0S416 93.1 416 208zM208 352a144 144 0 1 0 0-288 144 144 0 1 0 0 288z"
				/>
			</svg></button
		>
		<!-- </div> -->
	</svelte:fragment>
</AppBar>
