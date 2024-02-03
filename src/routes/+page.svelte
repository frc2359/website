<script>
	import gsap from "gsap";
	import SiteHeader from "../components/SiteHeader.svelte";
	// @ts-ignore
	import Carousel from 'svelte-carousel';
	import { onMount } from "svelte";
	import ScrollTrigger from 'gsap/dist/ScrollTrigger';
	import { browser } from "$app/environment";

	gsap.registerPlugin(ScrollTrigger);

	onMount(() => {
		if(browser) {
			gsap.from('#mark', {fontSize: '15vh'});
			gsap.from('#markimg', {width: '45vw'});
			gsap.from('.carou_img', {filter: 'blur(20px)'});

			gsap.timeline({
				scrollTrigger: {
					trigger: '.first',
					start:'top top',
					end:'bottom bottom',
					endTrigger: '#hero1',
					scrub: 1
				}
			})
			.to('#mark', {fontSize: '15vh'}, 0)
			.to('#markimg', {width: '45vw'}, 0)
			.to('.carou_img', {filter: 'blur(20px)'}, 0)
		}
	});

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
		<h1 id='mark'>WE ARE <span><img id='markimg' src="../rbolobo_wh_cl.svg" alt="logo"></span></h1>
	</div>
	
	<div class="second">
		<h1><span>One</span> step at a time</h1>
		<p>Resillence, inginuity, teamwork, effort. Our goal is to create a commnuity of students prepared to tackle the challenges of tomorrow, from the ground up.
			 3 months, one robot. Are you ready?</p>
		<div class="sizzle">
			<div class="item">
				<span class="material-symbols-outlined">
					diversity_3
				</span>
				<p>Teamwork Skills</p>
			</div>
			<div class="item">
				<span class="material-symbols-outlined">
					engineering
				</span>
				<p>Engineering Skills</p>
			</div>
			<div class="item">
				<span class="material-symbols-outlined">
					flag
				</span>
				<p>Workforce Development</p>
			</div>
		</div>
			
		<img src="../images/sidebyside.jpg" alt="">
	</div>

	<div class="third" id='sponsors'>
		<h1>Making it <span>possible</span></h1>
		<p>Sponsors help support us, and make everything we do possible.</p>
		<div class="sponsorimgs">
			<p>Coming soon!</p>
			<!-- <img src="../images/boeing.png" alt="">
			<img src="../images/raytheon.png" alt="">
			<img src="../images/Reversed_DoDSTEM_Logo.png" alt=""> -->
		</div>
		
	</div>

</div>

<style>
	.page {
		margin-top: 12vh;
	}
	h1 span {
		color: var(--green-200);
	}
	p {
		line-height: 1.5;
		font-size: 2.5vh;
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
	.first #markimg {
		width: 30vw;
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
		grid-template-rows: 20vh 70vh;
	}
	.second h1, .third h1 {
		grid-row: 1;
		grid-column: 1;
		padding-top: 5vh;
		padding-left: 4vw;
	}
	.second > p {
		grid-row: 2;
		grid-column: 1;
		padding-left: 4vw;
		line-height: 1.5;
		font-size: 2.5vh;
	}
	.second > .sizzle {
		grid-row: 2;
		grid-column: 1;
		align-self: center;
		justify-self: center;
		/* background-color: green; */
		width: 40vw;
		text-align: center;
		height: 20vh;
		display: flex;
		flex-direction: row;
		justify-items: space-between;
	}
	.second > .sizzle > .item {
		display: flex;
		/* background-color: #8a5151; */
		padding-left: 2vw;
		padding-right: 2vw;
		width: calc(40vw/3);
		flex-direction: column;
		justify-content: center;
		justify-items: center;
		align-items: center;
		border-right: 2px solid rgb(87, 87, 87);
	}
	.second > .sizzle > .item:last-child {
		border-right: 0px solid white;

	}
	.second > .sizzle > .item > span {
		font-size: 10vh;
		color: var(--green-200);
		justify-self: center;
	}
	.second > .sizzle > .item > p {
		font-size: 2.5vh;
		justify-self: center;
	}
	.second > img {
		grid-row: 1/ span 2;
		grid-column: 2;
		width: 45vw;
		object-fit: cover;
		height: 90vh;
		justify-self: end;
	}
	.third {
		height: 60vh;
	}
	.third > p {
		padding-left: 4vw;
	}
	.third .sponsorimgs {
		height: 40vh;
		padding-left: 5vw;
		width: 90vw;
		display: flex;
		flex-wrap: wrap;
		justify-content: space-between;
	}
	.third .sponsorimgs > img {
		height: 20vh;
	}
</style>