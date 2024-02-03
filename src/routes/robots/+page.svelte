<script>
	import SiteHeader from "../../components/SiteHeader.svelte";
	import Card from "../../components/Card.svelte";
</script>

<SiteHeader></SiteHeader>

<div class="page">
<Card />
<Card name='Spike' year="Charged Up" image="../images/_MG_8775.JPG" accolades="{`1st - Kansas City Regional<br>3rd - Oklahoma Regional<br>3rd - Green Country Regional`}"/>
</div>

<style>
	.page {
		margin-top: 15vh;
		display: flex;
		width: 90vw;
		padding-left: 5vw;
		flex-direction: row;
		flex-wrap: wrap;
		justify-content: space-around;
	}
	
</style>