<script>
	import Counter from './Counter.svelte';
	import welcome from '$lib/images/svelte-welcome.webp';
	import welcome_fallback from '$lib/images/svelte-welcome.png';
	import { Section, News, HeroHeader, HeroBody } from 'flowbite-svelte-blocks';
	import { Alert, Button } from 'flowbite-svelte';
	import { ArrowRightOutline } from 'flowbite-svelte-icons';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section
	class="bg-[url('https://firebasestorage.googleapis.com/v0/b/holonconsulting-9064d.appspot.com/o/main_bg.jpg?alt=media&token=4f37d5c1-342f-4887-9998-93c413fe8c49')] bg-cover bg-no-repeat bg-blend-multiply"
>
	<div class="col-lg-12 section-title fadeIn wow">
		<div class="uppercase"><strong></strong></div>

		<div class="title-bar dark-bg"></div>
		<h1 class=" uppercase">Value Delivered:</h1>
		<div class="textcenter info-text">
			<ul>
				<li style="font-size:18px;">31% reduction in operational costs for a mid-size bank</li>
				<li style="font-size:18px;">66% unit cost reduction by eliminating waste</li>
				<li style="font-size:18px;">
					50% increase in processing capacity <br />
					(through creation of a shared services environment)
				</li>
				<li style="font-size:18px;">40% reduction in Turn-Around-time</li>
			</ul>
		</div>
	</div>

	<!-- <Counter /> -->
	<div class="homepage_cirlce_wchdfy">What can <br /> Holon Consulting <br /> do for you?</div>
	<div class="row section1">
		<div class="main_circle_section">
			<div class="homepage_cirlce" style="background-color: rgb(239, 120, 55);">
				<a href="strategyConsulting.html">Strategy Consulting</a>
			</div>
			<div class="homepage_cirlce" style="background-color: rgb(38, 140, 197);">
				<a href="businessAnalysis.html">Business Analysis</a>
			</div>
			<div class="homepage_cirlce bpm" style="background-color: rgb(112, 191, 151);">
				<a href="businessProcessManagement.html">Business Process Management</a>
			</div>
			<div class="homepage_cirlce" style="background-color: rgb(248, 190, 59);">
				<a href="executiveCoaching.html">Executive Coaching</a>
			</div>
		</div>
	</div>
</section>

<!--  -->

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 1;
	}

	h1 {
		width: 100%;
	}
	.home {
		background-image: 'https://firebasestorage.googleapis.com/v0/b/holonconsulting-9064d.appspot.com/o/main_bg.jpg';
	}
	.welcome {
		display: block;
		position: relative;
		width: 100%;
		height: 0;
		padding: 0 0 calc(100% * 495 / 2048) 0;
	}

	.welcome img {
		position: absolute;
		width: 100%;
		height: 100%;
		top: 0;
		display: block;
	}
	.homepage_cirlce_wchdfy {
		position: absolute;
		background-color: rgba(255, 0, 0, 0.5);
		color: #fff;
		height: 250px;
		width: 250px;
		border-radius: 200px;
		text-align: center;
		font-size: 1.8em;
		padding-top: 60px;
		right: 13%;
		top: 41%;
	}
	.homepage_cirlce_wchdfy_small {
		position: absolute;
		color: #fff;
		height: 50px;
		width: 50px;
		border-radius: 50px;
		text-align: center;
		font-size: 1.8em;
		padding-top: 42px;
		right: 20%;
		top: 64%;
		z-index: 9;
		background-color: rgba(255, 0, 0, 0.5);
	}
	.homepage_cirlce {
		height: 200px;
		width: 200px;
		border-radius: 200px;
		background-color: #fff;

		margin: 20px 40px;
	}
	.homepage_cirlce:hover {
		height: 195px;
		width: 195px;
	}
	.homepage_cirlce a,
	.homepage_cirlce_wchdfy a {
		display: block;
		width: 100%;
		height: 100%;
		text-align: center;
		padding: 70px 10px 0px 10px;
		font-size: 1.5em;
	}
	.main_circle_section {
		position: absolute;
		display: flex;
		flex-direction: row;
		width: 100%;
		bottom: 0%;
		left: 0;
		right: 0;
		height: 300px;
		background-color: #fff;
	}
	.main_circle_section a {
		color: #fff;
	}
</style>
