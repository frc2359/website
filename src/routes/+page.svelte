<script>
	import SiteHeader from "../components/SiteHeader.svelte";
	// @ts-ignore
	import Carousel from 'svelte-carousel';

</script>
<SiteHeader></SiteHeader>

<div class="page">
	<div class="first">
		<Carousel autoplay autoplayDuration={5000} autoplayProgressVisible pauseOnFocus arrows={false}>
			<img src="../images/IMG_4565.JPG" class="carou_img" alt="">
			<img src="../images/_MG_9155.JPG" class="carou_img" alt="">
			<img src="../images/_MG_9316.JPG" class="carou_img" alt="">
			<img src="../images/_MG_9042.JPG" class="carou_img" alt="">
		</Carousel>
		<h1>WE ARE <span><img src="../rbolobo_wh_cl.svg" style="width: 30vw" alt="logo"></span></h1>
	</div>
	
	<div class="second">
		<h1><span>ONE</span> step at a time</h1>
		<p>Resillence, inginuity, teamwork, effort. Our goal is to create a commnuity of students prepared to tackle the 
			challenges of tomorrow, from the ground up. 3 months, one robot. Are you ready?</p>
		<img src="../images/_MG_9558.JPG" class="carou_img" alt="">
	</div>

</div>

<style>
	.page {
		margin-top: 12vh;
	}
	h1 span {
		color: var(--green-200);
	}
	.first {
		margin: 0;
		padding: 0;
		display: flex;
		
	}
	.first h1 {
		position: absolute;
		font-size: 10vh;
		/* font-weight: 90; */
		margin-top: 30vh;
		width: 100vw;
		text-align: center;

	}
	.carou_img {
		max-height: 90vh;
		max-width: 100vw;
		background-size: cover;
		object-fit: cover;
		opacity: 0.3;
	}
	.second{
		display: grid;
		grid-template-columns: 50vw 50vw;
		grid-template-rows: 10vh 80vh;
	}
	.second h1 {
		grid-row: 1;
		grid-column: 1;
	}
	.second > p {
		grid-row: 2;
		grid-column: 1;
		font-size: 2.5vh;
	}
	.second > img {
		grid-row: 1/ span 2;
		grid-column: 2;
		width: 20vw;
		height: 90vh;
		justify-self: end;
	}
</style>