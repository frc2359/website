<script>
	import SiteHeader from "../components/SiteHeader.svelte";
	// @ts-ignore
	import Carousel from 'svelte-carousel';

</script>
<SiteHeader></SiteHeader>

<div class="page">
	<Carousel let:showPrevPage let:showNextPage>
		<!-- svelte-ignore a11y-no-static-element-interactions -->
		<!-- svelte-ignore a11y-click-events-have-key-events -->
		<div slot="prev" on:click={showPrevPage} class="custom-arrow custom-arrow-prev">
			<span class="material-symbols-outlined">
				arrow_back_ios
			</span>
		</div>

		

		<!-- svelte-ignore a11y-click-events-have-key-events -->
		<!-- svelte-ignore a11y-no-static-element-interactions -->
		<div slot="next" on:click={showNextPage} class="custom-arrow custom-arrow-next">
			<span class="material-symbols-outlined">
				arrow_forward_ios
			</span>
		</div>
	</Carousel>

</div>

<style>
	.page {
		margin-top: 20vh;
	}
	.material-symbols-outlined {
		font-variation-settings:
		'FILL' 0,
		'wght' 400,
		'GRAD' 0,
		'opsz' 24
	}
</style>