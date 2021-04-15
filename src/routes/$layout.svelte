<script>
	// import 'bulma/css/bulma.css';
	import icons from '$lib/icons.js';
</script>

<svelte:head>
	<link rel="stylesheet" href="/css/bulma.css" />
	<link rel="stylesheet" href="/css/main.css" />
</svelte:head>

<svg
	aria-hidden="true"
	style="position: absolute; width: 0; height: 0; overflow: hidden;"
	version="1.1"
	xmlns="http://www.w3.org/2000/svg"
	xmlns:xlink="http://www.w3.org/1999/xlink"
>
	<defs>
		<!--
 * Font Awesome Free 5.12.1 by @fontawesome - https://fontawesome.com
 * License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License)
            -->
		{#each icons as icon}
			<symbol id={icon.id} viewBox={icon.viewBox}>
				<title>{icon.title}</title>
				<path d={icon.path} />
			</symbol>
		{/each}
	</defs>
</svg>
<nav class="navbar" role="navigation" aria-label="main navigation">
	<div class="navbar-menu is-active">
		<div class="navbar-start">
			<a class="navbar-item has-text-weight-light is-size-5" href="."> Home </a>

			<a class="navbar-item has-text-weight-light is-size-5" href="/model"> Supply & Demand </a>
			<a class="navbar-item has-text-weight-light is-size-5" href="/diffusion"> Diffusion </a>

			<a class="navbar-item has-text-weight-light is-size-5" href="/documentation">
				Documentation
			</a>

			<a class="navbar-item has-text-weight-light is-size-5" href="/publications"> Publications </a>
		</div>
	</div>
</nav>

<slot />

<section class="section has-background-white-er is-bold">
	<h1 class="title center is-spaced has-text-weight-light">Explore</h1>
	<div class="container">
		<div class="columns">
			<div class="column">
				<article class="media notification is-link" style="height:100%;">
					<figure class="media-left">
						<span class="icon is-medium">
							<svg>
								<use xlink:href="#chart-line" />
							</svg>
						</span>
					</figure>
					<div class="media-content">
						<div class="content">
							<h1 class="title has-text-weight-light is-size-4">Supply & Demand</h1>
							<p class="is-size-5">
								Want to learn about the future supply and demand of our state's licensed practical
								nurses and registered nurses across settings and geographic regions?
							</p>
							<a class="button is-warning is-outlined is-center is-rounded" href="/model">
								<strong class="has-text-weight-semibold">Select here</strong>
							</a>
						</div>
					</div>
				</article>
			</div>

			<div class="column">
				<article class="media notification is-link" style="height:100%;">
					<figure class="media-left">
						<span class="icon is-medium">
							<svg>
								<use xlink:href="#graduation-cap" />
							</svg>
						</span>
					</figure>
					<div class="media-content">
						<div class="content">
							<h1 class="title has-text-weight-light is-size-4">Program Diffusion</h1>
							<p class="is-size-5">
								Want to see how different North Carolina nursing programs impact the distribution of
								health professionals in their area and across the state?
							</p>

							<a class="button is-warning is-outlined is-center is-rounded" href="/diffusion">
								<strong class="has-text-weight-semibold">Select here</strong>
							</a>
						</div>
					</div>
				</article>
			</div>
			<div class="column">
				<article class="media notification is-link" style="height:100%;">
					<figure class="media-left">
						<span class="icon is-medium">
							<svg>
								<use xlink:href="#file-alt" />
							</svg>
						</span>
					</figure>
					<div class="media-content">
						<div class="content">
							<h1 class="title has-text-weight-light is-size-4">Documentation</h1>
							<p class="is-size-5">
								Are you a data-oriented individual? Want to learn more about our model and
								methodology, basic nursing statistics, and the science behind our work?
							</p>

							<a class="button is-warning is-outlined is-center is-rounded" href="/documentation">
								<strong class="has-text-weight-semibold">Select here</strong>
							</a>
						</div>
					</div>
				</article>
			</div>
		</div>
	</div>
</section>

<section class="section has-background-light is-bold">
	<div class="container">
		<div class="columns">
			<div class="column is-8-desktop is-offset-2-desktop">
				<h1 class="title center is-spaced has-text-weight-light">Who are we?</h1>
				<h2 class="subtitle">
					This project is brought to you by The Cecil G. Sheps Center For Health Services Research
					at the University of North Carolina in partnership with the North Carolina Board of
					Nursing.
				</h2>
			</div>
		</div>
	</div>
</section>

<footer class="footer has-background-warning">
	<div class="container">
		<div class="columns">
			<div class="column is-8-desktop is-offset-2-desktop">
				<div class="columns">
					<div class="column is-one-third">
						<div class="column">
							<figure class="image">
								<img src="/images/NCBNlogo.svg" alt="North Carolina Board of Nursing Logo" />
							</figure>
						</div>
						<div class="column">
							<figure class="image">
								<img src="/images/workforce.svg" alt="Logo of Sheps Health Workforce NC" />
							</figure>
						</div>
					</div>
					<div class="column has-text-right">
						<p>
							<strong> Contact us </strong>
							<br />UNC Program on Health Workforce & Research
							<br /> Email: nchealthworkforce@unc.edu
							<br /> Phone: 919-966-5011
						</p>
					</div>
				</div>
			</div>
		</div>
	</div>
</footer>
